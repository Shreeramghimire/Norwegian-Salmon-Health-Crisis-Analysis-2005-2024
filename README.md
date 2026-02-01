# Norwegian Salmon Health Crisis: 20 Years of Disease vs Production Expansion (2005-2024)

## 📊 Executive Summary
This analysis examines two decades of disease surveillance in Norwegian Atlantic salmon aquaculture, revealing critical insights about the relationship between industrial expansion and fish health. Despite a 42.5% increase in production licenses, disease patterns show complex dynamics—some infections declined dramatically due to vaccines while others increased, highlighting both successes and ongoing challenges in sustainable aquaculture.

## 🎯 Project Objectives
1. **Quantify** the relationship between production expansion and disease incidence
2. **Evaluate** the impact of vaccine introductions on target diseases  
3. **Identify** emerging disease threats in modern salmon farming
4. **Provide** data-driven recommendations for sustainable aquaculture

## 📁 Dataset Overview
**Source:** Norwegian Directorate of Fisheries and Veterinary Institute  
**Period:** 2005-2024 (20 continuous years)  
**Records:** Annual disease case counts + production licenses  
**Diseases Tracked:** 8 major salmon pathogens  
**File:** `salmon_diseases_2005_2024.csv`

### Key Variables:
- **Production Indicator:** Annual operational licenses
- **Diseases Monitored:**
  - ISA (Infectious Salmon Anaemia)
  - IPN (Infectious Pancreatic Necrosis)
  - PD (Pancreas Disease)
  - HSMI (Heart and Skeletal Muscle Inflammation)
  - Furunculosis
  - BKD (Bacterial Kidney Disease)
  - CMS (Cardiomyopathic Syndrome)
  - Cold-water vibriosis

## 🔬 Methodology

### Data Processing Pipeline
1. **Data Cleaning:** Handle missing values, convert data types
2. **Feature Engineering:** Calculate derived metrics
3. **Exploratory Analysis:** Visual trends and correlations
4. **Statistical Modeling:** Regression and hypothesis testing
5. **Interpretation:** Translate findings into insights

### Analytical Techniques
- **Descriptive Statistics:** Temporal trends and distributions
- **Correlation Analysis:** Disease-disease and disease-license relationships
- **Regression Models:** Linear, polynomial, and regularized regression
- **Comparative Analysis:** Pre/post vaccine periods
- **Time Series Analysis:** Lag effects and temporal patterns

## 📈 Key Analyses Performed

### 1. Disease Trend Visualization
- Individual disease trajectories over 20 years
- Peak incidence identification for each pathogen
- Comparative burden assessment

### 2. Production-Disease Relationship
- License growth vs. disease incidence correlation
- Cases per license density metric
- Time-lagged effects analysis

### 3. Vaccine Impact Assessment
- IPN vaccine (introduced ~2012) effectiveness
- PD vaccine (introduced ~2017) outcomes
- Statistical significance testing of reductions

### 4. Multivariate Analysis
- Multiple regression: Total cases = f(Licenses, Year, Licenses²)
- Regularized regression for feature importance
- Residual diagnostics and model validation

##  Key Findings

### Success Stories:
- **IPN Dramatic Reduction:** Cases dropped from 200+ to <30 annually post-2012 vaccination
- **Effective Disease Management:** Overall cases per license trend shows improvement

### Emerging Concerns:
- **CMS Increase:** Steady rise from ~70 to 150+ cases despite controls
- **HSMI Variability:** Fluctuations suggest density-dependent challenges
- **Recent BKD Resurgence:** Increase in 2023-2024 warrants attention

### Production-Disease Insights:
- **Positive Correlation:** CMS and HSMI scale with production
- **Decoupled Success:** IPN reduced despite production growth (vaccine effect)
- **Mixed Patterns:** Other diseases show complex, non-linear relationships

##  Practical Implications

### For Salmon Farmers:
1. **Vaccine Priority:** Maintain IPN vaccination, consider PD vaccine adoption
2. **Density Management:** Monitor CMS and HSMI in high-density operations
3. **Surveillance Focus:** Enhanced monitoring for BKD resurgence

### For Policymakers:
1. **Vaccine Support:** Continue funding for effective immunization programs
2. **Sustainable Growth:** Balance production expansion with health safeguards
3. **Research Investment:** Target diseases without effective vaccines (CMS, BKD)

### For Industry Stakeholders:
1. **Risk Assessment:** Consider disease burden in expansion planning
2. **Technology Adoption:** Invest in advanced health monitoring systems
3. **Collaborative Solutions:** Industry-wide disease management strategies

##  Results Dashboard
The analysis generates multiple outputs:

### Visualizations:
1. `disease_trends.png` - Individual disease trajectories
2. `licenses_vs_cases.png` - Production-disease relationship
3. `correlation_heatmap.png` - Disease interrelationships
4. `disease_contribution.png` - Relative burden of each disease
5. Regression diagnostics and model visualizations

### Data Outputs:
1. `processed_salmon_diseases_data.csv` - Cleaned dataset with calculated metrics
2. `disease_summary_statistics.csv` - Aggregated statistics for each disease

## Limitations & Considerations

### Data Constraints:
- Licenses as production proxy (not actual biomass)
- Diagnostic improvements over time may affect case detection
- Environmental factors not included in analysis
- Possible underreporting in early years

### Analytical Limitations:
- Small temporal sample (n=20 years)
- Correlation does not imply causation
- Multiple confounding factors in real world setting
- No control group for natural experiment analysis


### Prerequisites:
```bash
Python 3.8+
Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels
