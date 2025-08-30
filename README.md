# Finance and the Unexpected – Paper & Appendix Code

**Authors:** Saranya Anantapantula & Jessica Wachter  

This repository accompanies the paper *Finance and the Unexpected* and contains the Python code, data, and supporting materials used to generate the simulations and empirical figures.

---

## Repository Structure

### Documents [`documents/`]
- [`FinanceAndTheUnexpected.pdf`](./FinanceAndTheUnexpected.pdf)  
  Draft of the main paper.  
- [`Appendix_PDF.pdf`](./Appendix_PDF.pdf)  
  PDF export of the main Jupyter notebook for easier viewing.  
- [`FinanceAndTheUnexpected_Latex/`](./documents/FinanceAndTheUnexpected_Latex/)  
  LaTeX source folder for the paper, including figures, bibliography file, and `.tex` files.

---

### Replication Package [`replication_package/`]
- [`README.md`](./replication_package/README.md)  
  Describes data availability, file structure, and replication instructions.  
- [`Appendix_Code.ipynb`](./replication_package/Appendix_Code.ipynb)  
  Main Jupyter notebook reproducing all appendix figures.  
- [`data/`](./replication_package/data/)  
  Contains CSV files (WRDS and CBOE) used for Figures 4, 5, 8, 13, and 14.  

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
