# Transport Services and Mobility Challenges in Kumasi Metropolitan Area, Ghana

**A Data Analysis Project**  
Lawrence Ankomah Sei · November 2025  


## Project Description
This project analyzes public transport services and mobility challenges in Kumasi, Ghana’s second-largest city. The dataset includes **393 passengers** and **339 transport operators (drivers)** surveyed across four major routes in 2025.

The analysis integrates descriptive statistics, inferential modeling (chi-square tests, logistic/linear/ordinal regression), and machine learning techniques (Random Forest, K-means clustering, PCA) to generate evidence-based insights into service quality, operational constraints, and passenger travel behavior.

## Research Objectives
1. Identify the range and characteristics of transport services in Kumasi  
2. Develop and assess a Service Quality Index (SQI)  
3. Examine major challenges faced by passengers and operators  
4. Analyze mobility constraints and how they affect vulnerable groups  

## Dataset
- **Passengers:** 393 respondents (53% female; modal age 26–35)  
- **Drivers:** 339 respondents (100% male; mostly trotros)  
- Data collected via structured questionnaires on four transport corridors  
- All shared data is anonymized and stored in `/data/`  
- **No personal identifiers included**

## Methods Used
- Descriptive statistics (summary tables with `kableExtra`)  
- Inferential statistics:  
  - Chi-square tests  
  - Independent samples t-tests  
  - Logistic, linear, and ordinal logistic regression  
- Reliability testing (Cronbach’s α)  
- Correlation matrices  
- Machine learning:  
  - Random Forest classification  
  - K-means clustering  
  - Principal Component Analysis (PCA)  
- Text mining of open-ended responses  
- All analyses completed in R (`tidyverse`, `caret`, `randomForest`, `corrplot`, `factoextra`, `wordcloud2`, etc.)

## Key Findings
- **Trotro** dominates urban transport (93.4%).  
- Service Quality Index (SQI) is **fair** (mean 2.37/4.0).  
- Major passenger issues: overcrowding (64%), waiting times (60%), high fares (49%).  
- **78%** of passengers report severe traffic congestion.  
- Drivers cite **indiscipline** and **poor traffic management** as key congestion drivers.  
- Random Forest model predicts mode switching with **73.1% accuracy**.  
- **Four passenger clusters** identified via K-means.  
- **85.5%** public support for improved systems (BRT, light rail).

---

##  Folder Structure

```plaintext
.
├── data/                           # Anonymized CSV files
├── Transport_Analysis.Rmd          # Main R Markdown file
├── Transport_Analysis.html / pdf   # Rendered output
└── README.md                       # This file
▶ How to Reproduce the Analysis
Clone the repository
git clone https://github.com/yourusername/kumasi-transport-analysis.git
Open the R Markdown file
Transport_Analysis.Rmd
Install required R packages (run once):
install.packages(c(
  "tidyverse", "kableExtra", "caret", "randomForest",
  "corrplot", "wordcloud2", "factoextra", "psych", "MASS"
))
Knit the R Markdown file
Click Knit → choose HTML or PDF
The full report (tables, figures, models) will be generated automatically
Author
Lawrence Ankomah Sei
BSc Statistics (KNUST)
Email: seiankomahlawrence@gmail.com
