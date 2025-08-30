# Replication Package for: Finance and the Unexpected

This replication package accompanies Saranya Anantapantula and Jessica Wachter. (forthcoming). "Finance and the Unexpected".


## Authors

- Saranya Anantapantula
- Jessica Wachter

# Data availability and provenance statements
### Statement about rights

The authors of the manuscript have legitimate access to and permission to use the data used in this manuscript.

### Summary of availability
- All data in figures generated **are** publicly available or simulated.

### Details on each data source

- The daily returns data used to support the findings of this study were from the WRDS repository. [[1](https://wrds-www.wharton.upenn.edu/)]. The data were collected by the authors. Datafiles: `fig4_SRPT.csv`, `fig5_AAPL.csv`, `fig8_MarketReturns.csv`
- Data on the PutWrite index were downloaded from the Cboe Index Dashboard. Data can be downloaded from https://www.cboe.com/us/indices/dashboard/put/, select "Performance", then download. A copy of the data is provided as part of this archive. The data are in the public domain. Datafile: `fig13_PutWriteReturns.csv`
# Description of programs/code

- The program `Appendix_Code.ipynb` generates all figures (specified below). All datasets are located in `/data` and are already coded into the program. One will only need to run the program.
- All figures have been stored in `/figures`. 
# List of tables and figures

The provided code reproduces:
- Selected figures in the paper, as explained and justified below.


| Figure #          | Program                  | Output file                      | Note                            |
|-------------------|--------------------------|----------------------------------|---------------------------------|
| Figure 1          | n.a. (no data)           |                                  ||
| Figure 2          | n.a. (no data)           |                                  ||
| Figure 3          | Appendix_code.ipynb      | fig_03.png                       | Simulation parameters from Backus et al. (2011)|
| Figure 4          | Appendix_code.ipynb      | fig_04.png                       | Data from CRSP (2025)           |
| Figure 5          | Appendix_code.ipynb      | fig_05.png                       | Data from CRSP (2025)           |
| Figure 6          | Appendix_code.ipynb      | fig_06.png                       ||
| Figure 7          | n.a. (no data)           |                                  ||
| Figure 8          | Appendix_code.ipynb      | fig_08.png                       | Data from CRSP (2022)           |
| Figure 9          | Appendix_code.ipynb      | fig_09.png                       | Simulation parameters from Backus et al. (2011)|
| Figure 10         | n.a. (no data)           |                                  ||
| Figure 11         | n.a. (no data)           |                                  ||
| Figure 12         | n.a. (no data)           |                                  | Source: Benzoni et al. (2011) & Seo and Wachter (2019)|
| Figure 13         | Appendix_code.ipynb      | fig_13.png                       | Data from CRSP (2022) & CBOE (2025)|
| Figure 14         | Appendix_code.ipynb      | fig_14.png                       | Data from CRSP (2022) & CBOE (2025)|
| Figure 15         | n.a. (no data)           |                                  | Source: Seo and Wachter (2018)|
| Figure 16         | n.a. (no data)           |                                  | Source: Greenwood and Shleifer (2014)|
| Figure 17         | n.a. (no data)           |                                  | Source: Greenwood and Nagel (2009)|
| Figure 18         | n.a. (no data)           |                                  | Source: Malmendier and Wachter (2021)|
| Figure 19         | n.a. (no data)           |                                  | Source: Binsbergen et al. (2023)|


# References

- David Backus, Mikhail Chernov, and Ian Martin. Disasters implied by equity index options. _The Journal of Finance_, 66(6):1969–2012, 2011.
- CRSP Daily Stock File. Daily returns for Sarepta Therapeutics, 1997 - 2024. _Wharton Research Data Services (WRDS)_, 2025.
- CRSP Daily Stock File. Daily returns for Apple, 1980 - 2024. _Wharton Research Data Services (WRDS)_, 2025.
- CRSP Daily Stock File Indexes. Daily returns on the market portfolio, 1988 - 2022. _Wharton Research Data Services (WRDS)_, 2022.
- Luca Benzoni, Pierre Collin-Dufresne, and Robert S Goldstein. Explaining asset pricing puzzles associated with the 1987 market crash. _Journal of Financial Economics_, 101 (3):552–573, 2011.
- Sang Byung Seo and Jessica A Wachter. Option prices in a model with stochastic disaster risk. _Management Science_, 65(8):3449–3469, 2019.
- CBOE. Cboe global indices: Put index, 2025. URL https://www.cboe.com/us/indices/dashboard/put/.
- Sang Byung Seo and Jessica A Wachter. Do rare events explain CDX tranche spreads? _The Journal of Finance_, 73(5):2343–2383, 2018.
- Robin Greenwood and Andrei Shleifer. Expectations of returns and expected returns. _The Review of Financial Studies_, 27(3):714–746, 2014.
- Robin Greenwood and Stefan Nagel. Inexperienced investors and bubbles. _Journal of Financial Economics_, 93(2):239–258, 2009.
- Ulrike Malmendier and Jessica A Wachter. Memory of past experiences and economic decisions. _Available at SSRN 4013583_, 2021.
- Jules Van Binsbergen, Sophia Hua, Jonas Peeters, and Jessica Wachter. Is the US a lucky survivor? A hierarchical bayesian approach. _The Journal of Finance_, 2023.