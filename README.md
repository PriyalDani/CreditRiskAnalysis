# CreditRiskAnalysis

## Project Overview
This project aims to address challenges in assessing creditworthiness in emerging markets where detailed credit histories are often unavailable. Using the **Home Credit Default Risk** dataset, we employ advanced data analysis and machine learning techniques to predict loan repayment behavior. The ultimate goal is to improve financial inclusion and provide lenders with reliable tools for credit risk evaluation.

## Team Members
- Megan McKenna
- Apurva Atalkar
- Ahhaan Badhwar
- Priyal Devanshu Dani
- Rashmi Rao

---

## Table of Contents
1. [Client and Problem Statement](#client-and-problem-statement)
2. [Dataset Description](#dataset-description)
3. [Data Warehouse Design](#data-warehouse-design)
4. [Data Preparation](#data-preparation)
5. [Data Exploration](#data-exploration)
6. [Data Analysis and Results](#data-analysis-and-results)
7. [Business Implications](#business-implications)
8. [Appendix](#appendix)

---

## Client and Problem Statement
**Client:** Home Credit - A global consumer finance provider.  
**Objective:** Improve creditworthiness assessment to enhance financial inclusion in underserved populations by leveraging alternative data and predictive models.

Challenges:
- Limited credit history for potential borrowers.
- Unsustainable loan terms leading to financial instability.

Our solution focuses on:
1. Expanding access to credit.
2. Reducing default rates through better risk evaluation.

---

## Dataset Description
The dataset comprises multiple tables with demographic, financial, and transaction data:
1. **Loan Application Fact Table**
   - Details about each loan application.
   - Key variables: Loan amount, income, annuity, repayment status.
2. **Dimensions** include:
   - Bureau: Previous credits from other financial institutions.
   - Credit Card Balance: Monthly balance details for credit cards.
   - Previous Applications: Records of prior loans.
   - Customers: Demographics, employment, and family details.

---

## Data Warehouse Design
- **Process:**
  - Fact Table: Loan Applications.
  - Dimensions: Bureau, Credit Card Balance, Customers, Previous Applications.
  - Transformations using Python and SSIS for:
    - Ratio calculations (e.g., Debt-to-Credit Ratio).
    - Outlier and missing data handling.
  - Final data loaded into **HomeCredit_DW_Group5** database.

---

## Data Preparation
Steps involved:
1. **Outlier Detection & Handling**:
   - Adjusted extreme values in `DAYS_EMPLOYED` and `AMT_INCOME_TOTAL`.
2. **Missing Value Imputation**:
   - Mean imputation for continuous variables.
   - New category "Data Not Available" for categorical attributes.
3. **Label Encoding** for categorical variables to optimize space.

---

## Data Exploration
Key insights include:
1. Gender analysis revealed that while more women apply for loans, men default at a higher rate.
2. Family status impacts default probability, with singles and separated applicants being higher risks.
3. Income band analysis shows defaults are concentrated in the middle-income range.

---

## Data Analysis and Results
- **Risk Assessment:** Younger applicants exhibit higher debt-to-credit ratios.
- **Loan Duration:** Longer durations for mortgages and credit cards; shorter for small loans.
- **Segmentation Analysis:** Education level and gender affect default rates.
- **Credit Trends:** High-interest borrowers identified within certain organizations.

---

## Business Implications
1. **Enhanced Risk Evaluation**: Incorporate non-traditional data for better lending decisions.
2. **Tailored Loan Solutions**: Products targeting younger demographics and low-skilled professionals.
3. **Customer Education**: Financial literacy campaigns to improve repayment behavior.
4. **Targeted Marketing**: Use demographic insights to design focused marketing strategies.

---

## Appendix
Screenshots and additional details about:
- Data warehouse tables.
- Data transformations and visualizations.

  Please refer to the MIS587_Group5_ProjectReport document
