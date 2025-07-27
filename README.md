# Finance and the Unexpected - Paper & Appendix Code

**Authors:** Saranya Anantapantula & Jessica Wachter  

This repository accompanies the paper (Finance and the Unexpected) and contains the Python code and data used to generate our simulations and empirical figures. 

---

## Contents of this Repository 

**Paper Draft**
- [`Finance_and_the_Unexpected.pdf`](./Finance_and_the_Unexpected.pdf) – the current draft of the paper itself.


**Appendix Code & Data**  
- **`notebooks/Appendix.ipynb`** – Main Jupyter notebook reproducing all appendix figures.  
- **`/data`** – CSV files for WRDS and CBOE data used in Figures 4, 5, 8, 13, and 14.  

---

## Simulation & Empirical Figures 

The notebook provides the code for the following figures in the Appendix:

| Figure | Description | Data Source |
| ------ | ----------- | ----------- |
| **3** | Return distribution for a single stock (jump-diffusion simulation) | Simulated |
| **4** | Return distribution for a small-cap stock (SRPT) | WRDS Daily Stock File |
| **5** | Return distribution for a large stock (AAPL) | WRDS Daily Stock File |
| **6** | Return distribution for a portfolio of 100 stocks | Simulated |
| **8** | Daily returns on the market portfolio | CRSP Daily Stock File Indexes |
| **9** | Sampling distribution for kurtosis (Monte Carlo simulation) | Simulated |
| **13** | Distribution of returns: Put-Write Index vs Market Portfolio | CRSP & CBOE |
| **14** | Outlier returns: Put-Write Index vs Market Portfolio | CRSP & CBOE |

---