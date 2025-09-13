# Finance and the Unexpected – Paper & Appendix Code

**Authors:** Saranya Anantapantula & Jessica Wachter  

This repository accompanies the paper *Finance and the Unexpected* and contains the Python code, data, and supporting materials used to generate the simulations and empirical figures. 

Extreme events in financial markets challenge traditional models built on volatility and normal distributions. Tail risks, model failures, and behavioral biases continue to drive persistent mispricing and systemic vulnerability. Prior research often relies on mean-variance frameworks, overlooking higher moments like skewness and kurtosis, as well as the limits of diversification under moral hazard. We use simulated jump-diffusion models, Monte Carlo experiments, and empirical return data to expose the underestimation of rare, severe shocks in asset pricing and in investor expectations. Option markets, credit derivatives, and debt instruments reveal embedded short-put-like structures that mask hidden risks. Behavioral insights from memory and context effects explain why investors lean on recent experience, misjudge tail probabilities, and fail to revise models even after crisis events. While short-term returns are marked by negative skewness and excess kurtosis, the long-run performance of public equities, enabled by regulation and broad risk-sharing, remains a surprising and underappreciated success.

---
## Repository Structure

### Documents [`documents/`]
- [`FinanceAndTheUnexpected.pdf`](./documents/FinanceAndTheUnexpected.pdf)  
  Draft of the main paper.  
- [`Appendix_PDF.pdf`](./documents/Appendix_PDF.pdf)  
  PDF export of the main Jupyter notebook for easier viewing.  
- [`FinanceAndTheUnexpected_Latex/`](./documents/FinanceAndTheUnexpected_Latex/)  
  LaTeX source folder for the paper, including figures, bibliography file (`.bib`), and `.tex` files.

---

### Replication Package [`replication_package/`]
- [`README.md`](./replication_package/README.md)  
  Describes data availability, file structure, and replication instructions.  
- [`Appendix_Code.ipynb`](./replication_package/Appendix_Code.ipynb)  
  Main Jupyter notebook reproducing all appendix figures.  
- [`data/`](./replication_package/data/)  
  Contains CSV files (WRDS and CBOE) used for Figures 4, 5, 8, 13, and 14.  
- [`figures/`](./replication_package/figures/)  
  PNG files of figures 4, 5, 8, 13, and 14.  

---

## How to Use
1. Clone or download this repository.  
2. Navigate to the `replication_package/` folder.  
3. Open `Appendix_Code.ipynb` in Jupyter Notebook (or Jupyter Lab) to reproduce the figures.  
4. Data required for specific figures can be found in `/data`.  

---

## Notes
- Ensure Python ≥ 3.9 is installed.  
- Core dependencies include `numpy`, `pandas`, `matplotlib`, `scipy`. See the notebook for import details.  
- The LaTeX folder can be compiled directly with `pdflatex` to rebuild the paper.  
