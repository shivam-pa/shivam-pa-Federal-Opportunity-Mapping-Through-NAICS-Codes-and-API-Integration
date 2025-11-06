# Project: Federal Opportunity Mapping Through NAICS Codes and API Integration  
**Sponsor:** ImEx Cargo  
**Author:** Shivam Patel, Surya Devrath, Narasimha Singireddy

---

## Project Structure  
`Federal Opportunity Mapping Through NAICS Codes and API Integration/`  
```
├── data/          # Cleaned datasets and NAICS reference  
├── src/           # R scripts (data cleaning, NLP mapping, API integration)  
├── dashboards/    # Power BI dashboard (.pbix)  
└── docs/          # Final report (PDF)  
```

---
## Methods  

**Data Cleaning & Transformation:**  
R (tidyverse, dplyr, stringr) used for handling nulls, standardizing columns, and normalizing agency and NAICS fields.  

**Keyword → NAICS Mapping:**  
NLP preprocessing (tokenization, lemmatization) and TF-IDF filtering applied to map business or grant-related keywords to corresponding NAICS codes.  

**API Integration:**  
Grants.gov API integrated via `httr` and `jsonlite` in R to fetch live federal opportunity data based on NAICS classifications.  

**Visualization:**  
Interactive dashboard developed in Power BI (.pbix) to visualize NAICS distributions, agency funding, and mapped opportunities.  

---

## Deliverables  

- **docs/federal_opportunity_report.pdf** – Final APA-style report  
- **dashboards/federal_dashboard.pbix** – Power BI dashboard  
- **src/federal_mapping.R** – R code for data cleaning, NLP mapping, and API integration  
- **data/** – Cleaned CSVs and NAICS reference datasets

## How to Reproduce  

1. **Clone this repo:**
2. **Install required R packages:**
   ```R
   install.packages(c("tidyverse", "stringr","jsonlite","httr"))
   ```
3. **Run the R script:**
   - Open `src/federal_mapping.R` in RStudio.  
   - Ensure CSV/XLSX files from `data/` are in the working directory.  
   - Run the script to:
     - Clean and preprocess datasets  
     - Map keywords to NAICS codes  
     - Integrate live Grants.gov API data
4. **Open the Power BI dashboard:**  
   - Launch `dashboards/federal_dashboard.pbix` in **Power BI Desktop**.  
   - Interact with visuals to explore mapped opportunities and funding summaries.
  
---

## Outcomes  

- 45+ NAICS codes mapped  
- Grants.gov API successfully integrated  
- Clean and reproducible datasets  
- Interactive dashboard for opportunity insights  
- Final report summarizing project findings for stakeholders  

--- 
