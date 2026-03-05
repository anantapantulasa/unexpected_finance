# Finance and the Unexpected — Planning Notes

**Authors:** Saranya Anantapantula & Jessica Wachter
**Target journal:** Journal of Portfolio Management (JPM)
**Date:** March 5, 2026

---

## Current Manuscript

The most recent version of the LaTeX source is in:
`documents/FinanceAndTheUnexpected_Latex/`

This version (as opposed to the top-level `FinanceAndTheUnexpectedLATEX/` folder) includes:
- Abstract enabled
- Corrected skewness language ("shifts the mean above the median")
- Updated kurtosis values (19.8 for simulated individual stock; 15 for Monte Carlo threshold)
- Fixed citation syntax (`\citet` → `\citep` in several places)
- Added paragraph on Sarepta's kurtosis of 248
- Figure captions now include source citations (Figs. 12, 15)
- Year field added to CBOE reference

The compiled PDF is: `documents/FinanceAndTheUnexpected.pdf`

---

## Target Journal: JPM

JPM was founded by Peter Bernstein in 1974 as a bridge between academic finance and investment practice. It publishes thoughtful, accessible essays with mathematical substance — not theorem-proof papers. The journal accepts unsolicited submissions. The paper's narrative arc (theory → simulations → data → philosophical argument → surprising conclusion) fits JPM's editorial tradition well.

### Key precedents at JPM and related venues
- Peter Bernstein's own writings on risk (cf. *Against the Gods*)
- Andrew Lo & Mark Mueller, "Physics Envy May Be Hazardous to Your Wealth" (JOIM, 2010) — taxonomy of uncertainty, critique of Bayesian/frequentist frameworks in finance
- Itzhak Gilboa et al., "Probability and Uncertainty in Economic Modeling" (JEP, 2008) — directly questions the Bayesian assumption
- JPM's behavioral finance collection and tail risk management literature

---

## Ideas for Expansion and Revision

### 1. Moral Hazard Section — The Deeper Source of Uncertainty

The Holmström-Tirole model (Section 3) currently presents moral hazard as a problem where the agent acts strategically. On its face, this doesn't seem to connect to "the unexpected." The key insight to develop:

**The profound source of uncertainty in the real world is that you don't know whether you are facing a strategic or non-strategic agent.**

The current model assumes strategic behavior. But in reality, investors face uncertainty about the *type* of counterparty — are they honest or dishonest, competent or incompetent, strategic or naïve? This is a deeper form of uncertainty than what the model captures.

#### Connections to develop:
- **Glosten-Milgrom (1985):** The bid-ask spread model uses non-strategic ("noise") traders as a solution — informed traders can only profit because uninformed traders provide liquidity. Yet the model assumes the market maker knows the proportion of informed vs. uninformed traders. In reality, that proportion is itself uncertain.
- **Kyle (1985):** Similarly relies on noise traders to make the model tractable. The informed trader's strategy depends on the presence of non-strategic participants. Again, the true uncertainty — *how much* of the order flow is informed — is deeper than the model acknowledges.
- Both models use the non-strategic agent as a modeling device, but both also understate the true uncertainty by treating the mix of strategic/non-strategic agents as known.
- **Jessica's prior writing on this topic:** [Link to be added — Jessica to provide]

### 2. Bayesian Updating Example — Types of Uncertainty

Develop a careful, worked example illustrating different types of uncertainty through Bayesian updating. The key subtlety:

**A parameter might be fixed and yet unknown.**

This is the distinction between:
- **Risk:** The parameter is known (e.g., a fair coin — you know p = 0.5)
- **Uncertainty about a fixed parameter:** The parameter exists and is fixed, but you don't know it (e.g., a biased coin — p is some fixed value you must learn from data)
- **Deep/Knightian uncertainty:** You don't even know the right model or parameter space (e.g., the coin might have more than two sides, or it might not be a coin at all)

The Bayesian framework handles the second case elegantly but breaks down at the third. The paper's chicken problem is fundamentally about the third case — no amount of Bayesian updating on a misspecified model will save you.

#### Progression to develop:
- **Start with Akerlof's lemons problem (1970):** This is a clean, familiar Bayesian case. Buyers update beliefs about car quality based on the seller's willingness to sell. The uncertainty is well-defined: the quality is a fixed parameter, and the model is correct. People understand this case.
- **Move to a case where things get confusing:** Show how the same Bayesian apparatus breaks down when the model itself might be wrong — when you don't know whether you're in a lemons world or some other world entirely.
- **The power of the progression:** Going from a case people are comfortable with (Akerlof) to one where intuition fails makes the philosophical point concrete.

### 3. Kahneman and Tversky — People Don't Do Bayesian Updating

Integrate discussion of K&T's experimental findings showing systematic departures from Bayesian reasoning:
- Base rate neglect
- Representativeness heuristic
- Anchoring

This connects to the Section 6 discussion of memory and context effects but provides a more direct bridge: even in cases where Bayesian updating is the right framework, people fail to do it. Combined with the argument that the framework itself has limits (the chicken problem), this creates a two-pronged critique:
1. The Bayesian framework breaks down for tail risk and model uncertainty
2. Even where it doesn't break down, people don't follow it anyway

### 4. Integration of Lo & Mueller ("Physics Envy") and Gilboa et al.

The paper shares significant intellectual territory with these works and should engage with them explicitly:

- **Lo & Mueller:** Proposed a five-level taxonomy of uncertainty (complete certainty → risk → fully reducible uncertainty → partially reducible uncertainty → irreducible uncertainty). The paper's argument maps onto this taxonomy — the chicken problem lives at levels 4–5, but standard models assume level 2. Discuss how this paper's contribution differs: it provides *concrete financial examples* (put-writing, CDX tranches, hidden kurtosis) that illustrate what these abstract uncertainty levels look like in practice.
- **Gilboa et al.:** Directly questions whether probability is always the right language for uncertainty. The paper should engage with this — the hidden kurtosis result is a case where probability *exists* but cannot be reliably estimated. The chicken problem is a case where the probability model itself may be wrong.

### 5. Other Potential Additions (Lower Priority)
- Expand reference list significantly (currently 17 citations; JPM pieces typically cite more broadly)
- Consider whether the long-run equity success story (Section 7) needs more development as the "positive unexpected"
- Tighten the connection between Section 6 (memory/context) and the earlier sections

---

## Structural Notes

The current paper has a natural flow that works well:

1. **Introduction** — What is "the unexpected"?
2. **Individual stocks** — Wild, skewed returns
3. **Diversification** — Tames the wildness... but requires solving moral hazard
4. **Moral hazard** — Why diversification is limited in practice → *expand here*
5. **Aggregate returns** — Still fat-tailed; kurtosis is hidden
6. **Options & tail risk** — The chicken problem in multiple guises
7. **Discussion** — Why people fall for it (behavioral/memory)
8. **Conclusion** — The biggest surprise is positive

The new material could fit as follows:
- **Bayesian updating example:** Could go in a new subsection within the Introduction (Section 1), or as a new Section 2 that sets up the framework before diving into data
- **Glosten-Milgrom / Kyle / strategic vs. non-strategic:** Expand within Section 3 (Moral Hazard)
- **Kahneman & Tversky:** Integrate into Section 6 (Discussion), before the memory/context material
- **Lo, Gilboa engagement:** Could be woven throughout, or discussed in the Introduction/Conclusion

---

## Formatting To-Do for JPM Submission
- Look up JPM's specific submission guidelines (page limits, reference style, figure formatting)
- Adapt LaTeX document class and bibliography style
- Ensure all figures meet JPM's resolution and formatting requirements
- Write/revise abstract for JPM audience (more practitioner-facing)

---

## Open Items
- [ ] Jessica to provide link to her prior writing on strategic vs. non-strategic uncertainty
- [ ] Decide on placement of Bayesian updating example within the paper structure
- [ ] Decide how much to expand the moral hazard section vs. keeping it concise
- [ ] Review Gilboa et al. (2008) and Lo & Mueller (2010) for specific points to engage with
- [ ] Check JPM submission guidelines and formatting requirements
