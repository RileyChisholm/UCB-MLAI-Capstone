# **Analysis of Urbanization Impact on Local Climate Patterns and Air Quality**

**Author: Riley Chisholm**

---

### Executive Summary

This project explores the relationship between urban population growth, weather patterns, and air quality across major U.S. cities. Using a combination of linear regression, SARIMA time series analysis, and K-means clustering, the study aims to identify trends, correlations, and factors influencing urban climate and air quality. The results suggest that while population growth has some impact, it is not the sole determinant of these environmental factors. Local policies, environmental regulations, and geographical conditions also play crucial roles in shaping urban environments.

![Overview of cities analyzed](path_to_image1)

---

### Rationale

Understanding the factors that influence urban climate and air quality is crucial for city planners, policymakers, and public health officials. As urban populations continue to grow, the ability to predict and manage environmental outcomes becomes increasingly important. This analysis provides insights into how different cities manage these challenges and highlights the importance of local context in environmental outcomes. Effective planning and regulation can mitigate negative impacts, improving the quality of life for urban residents.

---

### Research Question

How has urbanization influenced local climate patterns, including temperature and air quality, in major US cities over the past 50 years?

---

### Data Sources

The study utilizes data from multiple sources:

- **US AQI Monthly Data:** Obtained from the Kaggle dataset ["US Air Quality Analysis"](https://www.kaggle.com/code/calebreigada/us-air-quality-analysis).
- **Weather Data:** Sourced from the National Centers for Environmental Information (NCEI).
- **Population Data:** Derived from the US Census, with interpolation for the years between official census counts to provide a continuous dataset.

---

### Methodology

This analysis employs several methods to explore the relationship between urbanization, temperature, and air quality:

1. **Linear Regression Analysis:** Examines the correlation between urban population growth and average temperature (TAVG) as well as AQI in major cities.
2. **SARIMA Time Series Analysis:** Decomposes temperature and AQI data to understand trends, seasonality, and long-term changes.
3. **K-means Clustering:** Groups cities based on their population and AQI characteristics, revealing patterns that suggest differing impacts of urbanization on air quality.

---

### Results

#### **Analysis of Weather Data Across Major U.S. Cities**

**Linear Regression Results**

The linear regression analysis aimed to explore the relationship between urban population growth and average temperature (TAVG) in various major U.S. cities. The results show considerable variation across different cities, indicating that the impact of population growth on temperature is not uniform.

- In cities like **San Antonio** and **Houston**, the linear regression models show a positive trend with relatively higher R-squared values, suggesting that population growth may have a more direct correlation with rising temperatures.

![SanAntonio(WLR)](https://github.com/user-attachments/assets/a340a993-4b35-4dcb-8baf-43180b9bc84a)
![Houston(WLR)](https://github.com/user-attachments/assets/84e0cc62-0073-4d55-bd90-604848240e74)


- However, in cities like **Los Angeles** and **San Diego**, negative R-squared values indicate that population growth alone does not account for temperature changes. This divergence suggests the influence of other factors, such as environmental regulations and urban planning, which may mitigate the temperature impacts of urbanization.

![LosAngeles(WLR)](https://github.com/user-attachments/assets/3ee6b3ce-580e-4f94-94ff-0f55186ce98b)
![SanDiego(WLR)](https://github.com/user-attachments/assets/45f09b83-5439-4662-8282-346fc8894b23)

**SARIMA Time Series Analysis**

The SARIMA (Seasonal Autoregressive Integrated Moving Average) models were used to analyze long-term temperature trends and seasonality.

- **New York** and **San Antonio** exhibited a clear upward trend in average temperatures, suggesting long-term warming potentially linked to urbanization and other local factors.

![NewYork(WSarima)](https://github.com/user-attachments/assets/4e76fcef-43ae-4d8f-97ea-8f4517c449ff)
![San Antonio(WSarima)](https://github.com/user-attachments/assets/d2990407-5278-4a79-9ea3-b09f79a4da0f)

- **San Diego** and **Los Angeles** did not show a consistent upward trend, indicating that these cities may have factors, such as green policies or geographic advantages, that help stabilize or reduce temperature increases despite population growth.

![San Diego(WSarima)](https://github.com/user-attachments/assets/ac1eca28-1c8f-4885-9c62-c97e2bab40bb)
![LosAngeles(WSarima)](https://github.com/user-attachments/assets/f852b4c5-4ed2-4f99-b2f8-8a6c509cc1fd)


#### **Air Quality Analysis Across Major U.S. Cities**

**Linear Regression Results**

The linear regression models aimed to examine the relationship between urban population growth and air quality, as measured by the AQI.

- In cities like **San Diego** and **Los Angeles**, the results indicate that as the population increases, AQI tends to improve. This counterintuitive result suggests that these cities may have implemented effective environmental regulations and policies that mitigate the impact of population growth on air quality. Factors such as investments in cleaner technologies, public transportation, and industrial regulations could be contributing to these trends.

![San Diego(AQLR)](https://github.com/user-attachments/assets/061a1302-54af-4c6f-bc11-c1b53c1d74d7)
![Los Angeles(AQLR)](https://github.com/user-attachments/assets/229cad92-92a1-410a-8aaf-01c793484422)

- Conversely, in cities like **Dallas** and **Jacksonville**, the low R-squared values suggest that population growth does not strongly predict changes in AQI. This could be due to effective air quality management practices or geographic conditions that help maintain air quality despite population increases.

![Dallas(AQLR)](https://github.com/user-attachments/assets/b38d9fef-8477-4278-8417-94e3d7ac07e4)
![Jacksonville(AQLR)](https://github.com/user-attachments/assets/b467bc96-5eeb-4ef3-93a0-7b7aa50ad68f)


**K-means Clustering**

The K-means clustering analysis provided insights into how cities group based on AQI and population characteristics.

- The analysis revealed that cities with higher populations do not necessarily have higher AQI levels. For example, **Phoenix** and **Houston** formed clusters with higher AQI levels, indicating challenges in managing air quality as populations rise, while **Seattle** and **San Diego** were clustered with lower AQI levels, suggesting effective air quality management or natural advantages such as geographic location.
- This reinforces the idea that factors beyond population, such as local environmental policies and geographic features, play crucial roles in determining air quality.

![Cluster](https://github.com/user-attachments/assets/ea9e8c10-f934-4ac1-ad17-87eeaf8d6412)

**SARIMA Time Series Analysis**

The SARIMA models were employed to understand the long-term trends and seasonality in AQI data across different cities.

- The SARIMA decomposition of the AQI data for **San Antonio** and **Phoenix** reveals upward trends in air quality index over the years, indicating a decline in air quality. This trend could be attributed to the rapid urbanization these cities have experienced, alongside other contributing factors such as increased industrial activities and vehicle emissions.

![San Antonio(AQSarima)](https://github.com/user-attachments/assets/764f5b42-ea66-4cec-9f75-787e094efa5a)
![Phoenix(AQSarima)](https://github.com/user-attachments/assets/6e964f65-5c09-4c1c-b065-18a1fffa7892)


- In contrast, the SARIMA decomposition for **New York** and **San Diego** shows more stable or even declining trends in AQI, suggesting that these cities have been successful in maintaining or improving air quality over time. This stability may result from effective air quality management practices, stringent environmental regulations, or beneficial geographic and climatic conditions that help mitigate pollution despite ongoing urban growth.

![NewYork(AQSarima)](https://github.com/user-attachments/assets/79151cb3-8a03-47c5-a571-e613297c0967)
![SanDiego(AQSarima)](https://github.com/user-attachments/assets/38a89535-373a-4037-9325-3438f47a9612)


---

### Next Steps

Based on the findings, the following next steps are recommended:

1. **Further Research:** Investigate the impact of specific environmental regulations on temperature and air quality outcomes in cities with varying trends.
2. **Policy Development:** Encourage the adoption of successful air quality management practices observed in cities like Seattle and San Diego.
3. **Advanced Modeling:** Incorporate additional variables such as industrial activity and transportation data to better understand the factors influencing urban climate and air quality.

---

### Outline of Project

- [Link to Notebook 1: Weather Data Analysis]()
- [Link to Notebook 2: Air Quality Analysis]()
- [Link to Notebook 3: Combined Clustering and Time Series Analysis]()


---

### Contact and Further Information

Riley Chisholm

Email: rileyrchisholm@gmail.com

[LinkedIn](https://www.linkedin.com/in/riley-chisholm-b1383521b/)

