# **Analysis of Urbanization Impact on Local Climate Patterns and Air Quality**

**Author: Riley Chisholm**

---

### Executive Summary

This project explores the relationship between urban population growth, weather patterns, and air quality across major U.S. cities. Using a combination of linear regression, SARIMA time series analysis, and K-means clustering, the study aims to identify trends, correlations, and factors influencing urban climate and air quality. The results suggest that while population growth has some impact, it is not the sole determinant of these environmental factors. Local policies, environmental regulations, and geographical conditions also play crucial roles in shaping urban environments.

![Overview of cities analyzed](path_to_image1)

---

### Rationale

Understanding the factors that influence urban climate and air quality is crucial for city planners, policymakers, and public health officials. As urban populations continue to grow, the ability to predict and manage environmental outcomes becomes increasingly important. This analysis provides insights into how different cities manage these challenges and highlights the importance of local context in environmental outcomes. Effective planning and regulation can mitigate negative impacts, improving the quality of life for urban residents.

![Graph or chart showing the importance of studying urban environments](path_to_image2)

---

### Research Question

How has urbanization influenced local climate patterns, including temperature and air quality, in major US cities over the past 50 years?

![Diagram or conceptual model illustrating the research question](path_to_image3)

---

### Data Sources

The study utilizes data from multiple sources:

- **US AQI Monthly Data:** Obtained from the Kaggle dataset "US Air Quality Analysis."
- **Weather Data:** Sourced from the National Centers for Environmental Information (NCEI).
- **Population Data:** Derived from the US Census, with interpolation for the years between official census counts to provide a continuous dataset.

![Screenshot or snippet of the data sources](path_to_image4)

---

### Methodology

This analysis employs several methods to explore the relationship between urbanization, temperature, and air quality:

1. **Linear Regression Analysis:** Examines the correlation between urban population growth and average temperature (TAVG) as well as AQI in major cities.
2. **SARIMA Time Series Analysis:** Decomposes temperature and AQI data to understand trends, seasonality, and long-term changes.
3. **K-means Clustering:** Groups cities based on their population and AQI characteristics, revealing patterns that suggest differing impacts of urbanization on air quality.

![Flowchart or diagram of the methodology steps](path_to_image5)

---

### Results

#### **Analysis of Weather Data Across Major U.S. Cities**

**Linear Regression Results**

The linear regression analysis aimed to explore the relationship between urban population growth and average temperature (TAVG) in various major U.S. cities. The results show considerable variation across different cities, indicating that the impact of population growth on temperature is not uniform.

- In cities like **San Antonio** and **Houston**, the linear regression models show a positive trend with relatively higher R-squared values, suggesting that population growth may have a more direct correlation with rising temperatures.
- However, in cities like **New York** and **San Diego**, negative R-squared values indicate that population growth alone does not account for temperature changes. This divergence suggests the influence of other factors, such as environmental regulations and urban planning, which may mitigate the temperature impacts of urbanization.

![Scatter plot with regression lines for TAVG vs. Population](path_to_image6)

**SARIMA Time Series Analysis**

The SARIMA (Seasonal Autoregressive Integrated Moving Average) models were used to analyze long-term temperature trends and seasonality.

- **New York** and **Jacksonville** exhibited a clear upward trend in average temperatures, suggesting long-term warming potentially linked to urbanization and other local factors.
- **Dallas** and **Los Angeles** did not show a consistent upward trend, indicating that these cities may have factors, such as green policies or geographic advantages, that help stabilize or reduce temperature increases despite population growth.

![SARIMA decomposition plot showing trend, seasonality, and residuals](path_to_image7)

#### **Air Quality Analysis Across Major U.S. Cities**

**Linear Regression Results**

The linear regression models aimed to examine the relationship between urban population growth and air quality, as measured by the AQI.

- In cities like **New York** and **Los Angeles**, the results indicate a more significant correlation between population and AQI, suggesting that population growth may contribute to worsening air quality due to factors like increased pollution from vehicles and industrial activities.
- Conversely, in cities like **San Antonio** and **Philadelphia**, the low R-squared values suggest that population growth does not strongly predict changes in AQI, possibly due to effective air quality management or favorable geographic conditions.

![Scatter plot with regression lines for AQI vs. Population](path_to_image8)

**K-means Clustering**

The K-means clustering analysis provided insights into how cities group based on AQI and population characteristics.

- The analysis revealed that cities with higher populations do not necessarily have higher AQI levels. For example, **Phoenix** and **Houston** formed clusters with higher AQI levels, indicating challenges in managing air quality as populations rise, while **Seattle** and **San Diego** were clustered with lower AQI levels, suggesting effective air quality management or natural advantages such as geographic location.
- This reinforces the idea that factors beyond population, such as local environmental policies and geographic features, play crucial roles in determining air quality.

![Clustering visualization (scatter plot) showing AQI vs. Population](path_to_image9)

**SARIMA Time Series Analysis**

The SARIMA models were employed to understand the long-term trends and seasonality in AQI data across different cities.

- **New York** and **Dallas** showed upward trends in AQI over the years, indicating a decline in air quality that could be linked to urbanization and other contributing factors.
- Meanwhile, cities like **Seattle** and **San Diego** exhibited more stable or even declining AQI trends, reflecting effective air quality management or other mitigating factors that help maintain or improve air quality despite urban growth.

![SARIMA forecast plot showing AQI trends](path_to_image10)

---

### Next Steps

Based on the findings, the following next steps are recommended:

1. **Further Research:** Investigate the impact of specific environmental regulations on temperature and air quality outcomes in cities with varying trends.
2. **Policy Development:** Encourage the adoption of successful air quality management practices observed in cities like Seattle and San Diego.
3. **Advanced Modeling:** Incorporate additional variables such as industrial activity and transportation data to better understand the factors influencing urban climate and air quality.

![Conceptual diagram or roadmap for future research](path_to_image11)

---

### Outline of Project

- [Link to Notebook 1: Weather Data Analysis]()
- [Link to Notebook 2: Air Quality Analysis]()
- [Link to Notebook 3: Combined Clustering and Time Series Analysis]()

![Overview or thumbnail image representing the notebooks](path_to_image12)

---

### Contact and Further Information

For more information or questions about this project, please contact Riley Chisholm at [Your Email Address]. Further details can be found on [Your GitHub Profile or LinkedIn].

