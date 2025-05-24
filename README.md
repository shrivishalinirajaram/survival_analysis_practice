# Survival Analysis Practice
This is a practice of survival analysis concepts on an existing dataset, analysis using R code and interpretation. Suggestions for improvement always welcome. 

---

## Repository Structure

<pre> ```text survival_analysis_practice/ ├── LICENSE ├── README.md ├── rendered_docs/ # Contains all the processed reports │ ├── Appendix_Rajaram.pdf │ ├── Codes_Rajaram_1.pdf │ ├── Codes_Rajaram.pdf │ └── Project_Rajaram.pdf ├── RMD/ # All the RMarkdown files for code, analysis, and interpretation │ ├── Appendix_Rajaram.rmd │ ├── Codes_Rajaram_1.rmd │ ├── Codes_Rajaram.rmd │ └── Project_Rajaram.rmd └── survival_analysis_practice.Rproj # RStudio project file ``` </pre>

---

## Document Descriptions

### `Project_Rajaram.rmd`  
**Main interpretive report**  
- Explores patient-level and clinical variables  
- Fits Kaplan-Meier curves, Cox models (time-independent and time-dependent), and AFT models (Weibull, Log-normal)  
- Includes PH assumption checks, functional form checks, and influence diagnostics  
- Tables and figures are generated using external scripts (from `Codes_Rajaram.rmd`)  
- Presents **tidy summaries, interpretation of outputs, and conclusions**  

### `Codes_Rajaram.rmd`  
**Code script for core analysis**  
- All code for:
  - Data preprocessing  
  - Model fitting (KM, Cox, AFT)  
  - Assumption diagnostics  
  - Summary tables and visualizations  
- Modularized and structured to support the main report (`Project_Rajaram.rmd`) and appendix

### `Appendix_Rajaram.rmd`  
**Supplementary outputs**  
- Additional figures and tables referenced in the main report  
- Includes diagnostics and stratified plots to support interpretation  
- All outputs generated from `Codes_Rajaram.rmd`

### `Codes_Rajaram_1.rmd`  
**Standalone full code notebook**  
- Contains **all code chunks used in `Codes_Rajaram`, `Project_Rajaram` and `Appendix_Rajaram`** in a single file  
- Suitable for full replication of the entire workflow  
- Does **not** include narrative interpretations

---

## Skills Demonstrated

- Survival analysis: KM curves, Cox PH models, AFT models  
- Time-varying covariates and PH assumption testing  
- Residual diagnostics and model validation  
- Tidyverse-based data processing and `broom`-style model outputs  
- Clean modular RMarkdown structure for reproducibility  
- Tidy tables (`gt`), visualizations (`ggplot2`), and interpretive scientific writing

---

## Rendered Reports

Available in the `rendered_docs/` folder:
- `Project_Rajaram.pdf`: Main interpretive analysis  
- `Codes_Rajaram.pdf`: Modular code and generation of outputs  
- `Appendix_Rajaram.pdf`: Additional plots, tables, and figures  
- `Codes_Rajaram_1.pdf`: Self-contained code-only notebook

---

## How to Use This Repository

1. Clone this repo and open `survival.Rproj` in RStudio  
2. Navigate to the `RMD/` folder  
3. Knit `Project_Rajaram.rmd` to produce the main report  
4. Use `Codes_Rajaram.rmd` to generate and update output tables/figures  
5. Use `Codes_Rajaram_1.rmd` as a full standalone code reference


