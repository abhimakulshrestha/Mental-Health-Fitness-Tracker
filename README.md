# Mental Health & Substance Use Disorder Data Analysis

A comprehensive Jupyter notebook analysis of global mental health and substance use disorder prevalence data. This project explores patterns, trends, and insights from mental health statistics across different countries and time periods.

## Project Overview

This data analysis project examines mental health and substance use disorders using two primary datasets:
- Mental and substance use disorders as a share of total disease burden
- Prevalence rates by specific mental health and substance use disorders

The analysis provides insights into global mental health trends, regional variations, and the relative impact of different mental health conditions.

## Dataset Information

### Dataset 1: Mental and Substance Use as Share of Disease
**File**: `mental-and-substance-use-as-share-of-disease.csv`
- **Description**: Mental and substance use disorders as percentage of total disease burden
- **Scope**: Global data across multiple years
- **Key Metrics**: Percentage share of overall disease burden

### Dataset 2: Prevalence by Mental and Substance Use Disorder
**File**: `prevalence-by-mental-and-substance-use-disorder.csv`
- **Description**: Age-standardized prevalence rates for specific mental health conditions
- **Scope**: Global data with country-level breakdowns
- **Disorders Covered**:
  - Schizophrenia
  - Bipolar disorder
  - Eating disorders
  - Anxiety disorders
  - Drug use disorders
  - Depressive disorders
  - Alcohol use disorders

### Data Structure
```
Columns in Dataset 2:
- Entity: Country/region name
- Code: Country code
- Year: Year of data collection
- Prevalence - [Disorder Name] - Sex: Both - Age: Age-standardized (Percent)
```

## Requirements

### Dependencies
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
```

### Installation
```bash
# Install required packages
pip install numpy pandas matplotlib seaborn plotly

# For Jupyter notebook
pip install jupyter

# Alternative: Install via conda
conda install numpy pandas matplotlib seaborn plotly jupyter
```

## Project Structure

```
mental-health-data-analysis/
│
├── Downloads/
│   └── data/
│       ├── mental-and-substance-use-as-share-of-disease.csv
│       └── prevalence-by-mental-and-substance-use-disorder.csv
│
├── mental_health_analysis.ipynb
├── README.md
└── requirements.txt
```

## Usage

### Getting Started
1. **Clone or download** the project files
2. **Ensure data files** are in the correct path: `Downloads/data/`
3. **Install dependencies** using pip or conda
4. **Launch Jupyter notebook**:
   ```bash
   jupyter notebook mental_health_analysis.ipynb
   ```

### Running the Analysis
Execute the notebook cells in order:

1. **Data Loading & Import**
   ```python
   import numpy as np
   import pandas as pd
   import matplotlib.pyplot as plt
   import seaborn as sns
   import plotly.express as px
   
   # Load datasets
   dataframe1 = pd.read_csv("Downloads/data/mental-and-substance-use-as-share-of-disease.csv")
   dataframe2 = pd.read_csv("Downloads/data/prevalence-by-mental-and-substance-use-disorder.csv")
   ```

2. **Data Exploration** - Examine dataset structure, missing values, and basic statistics
3. **Data Cleaning** - Handle missing values and standardize formats
4. **Exploratory Data Analysis** - Generate descriptive statistics and initial visualizations
5. **Trend Analysis** - Analyze temporal trends in mental health prevalence
6. **Comparative Analysis** - Compare prevalence across countries and disorders
7. **Visualization** - Create comprehensive charts and interactive plots

## Analysis Features

### Data Exploration
- Dataset overview and structure analysis
- Missing value assessment
- Statistical summaries for all disorders
- Data quality checks and validation

### Visualizations
- **Time Series Analysis**: Trends in mental health prevalence over time
- **Geographic Analysis**: Country-wise prevalence mapping
- **Comparative Charts**: Disorder prevalence comparison
- **Correlation Analysis**: Relationships between different disorders
- **Interactive Plots**: Plotly visualizations for dynamic exploration

### Key Metrics Analyzed
- Prevalence rates for 7 major mental health disorders
- Temporal trends and patterns
- Geographic distribution and hotspots
- Disorder co-occurrence patterns
- Disease burden analysis

## Expected Outputs

### Statistical Insights
- Global prevalence statistics for each disorder
- Identification of countries with highest/lowest prevalence
- Temporal trend analysis (increasing/decreasing patterns)
- Correlation coefficients between disorders

### Visualizations
- Line plots showing prevalence trends over time
- Heatmaps displaying correlation matrices
- Bar charts comparing prevalence across countries
- Geographic maps showing global distribution
- Interactive dashboards for data exploration

### Key Findings
The analysis will reveal:
- Which mental health disorders are most prevalent globally
- Geographic patterns in mental health prevalence
- Temporal trends in mental health statistics
- Relationships between different types of disorders
- Countries or regions requiring focused mental health interventions

## Data Sources

The datasets used in this analysis are sourced from reputable global health organizations and research institutions. The data includes:
- Age-standardized prevalence rates for accurate cross-country comparisons
- Multi-year data for trend analysis
- Comprehensive coverage of major mental health and substance use disorders

## Methodology

### Data Processing
- Data cleaning and standardization procedures
- Handling of missing values and outliers
- Age-standardization considerations
- Country code mapping and validation

### Analysis Approach
- Descriptive statistical analysis
- Time series analysis for trend identification
- Comparative analysis across countries and disorders
- Correlation analysis to identify relationships
- Geographic analysis for spatial patterns

## Limitations

### Data Limitations
- Reporting variations across countries
- Different healthcare system capabilities for diagnosis
- Cultural factors affecting mental health reporting
- Potential underreporting in certain regions

### Analysis Limitations
- Correlation does not imply causation
- Cross-sectional analysis limitations
- Country-level aggregation may mask regional variations
- Historical data availability varies by country

## Contributing

### How to Contribute
1. **Fork the repository** or download the notebook
2. **Add new analysis sections** or improve existing ones
3. **Include additional visualizations** or statistical tests
4. **Document your methodology** and findings
5. **Share insights** and recommendations

### Suggestions for Enhancement
- Additional statistical tests (ANOVA, regression analysis)
- Machine learning models for prediction
- Economic impact analysis
- Integration with demographic data
- Time series forecasting

## Applications

### Public Health
- Identify regions requiring mental health interventions
- Resource allocation for mental health services
- Policy development and planning
- Monitoring progress in mental health initiatives

### Research
- Academic research on global mental health trends
- Comparative studies across countries
- Hypothesis generation for further research
- Data-driven insights for mental health professionals

### Healthcare Planning
- Healthcare system capacity planning
- Professional training needs assessment
- Prevention program development
- Treatment resource allocation

## Technical Notes

### Performance Considerations
- Large datasets may require memory optimization
- Consider using data sampling for initial exploration
- Interactive plots may be slow with full datasets
- Optimize visualizations for better performance

### Reproducibility
- Set random seeds for consistent results
- Document package versions
- Include data preprocessing steps
- Save intermediate results for complex analyses


**Note**: This analysis is for research and educational purposes only. The findings should not be used as a substitute for professional medical advice or clinical decision-making.
