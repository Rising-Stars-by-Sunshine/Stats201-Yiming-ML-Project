# Harnessing Machine Learning for Understanding Global Energy and Predicting Renewable Energy Consumption Trends in Asia
## Project information
- **Author**:Yiming Yuan, Applied Mathematics and Computer Science, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for [STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I would like to thank Prof. Luyao Zhang for her detailed and enthusiastic instructions on machine learning methods and the constructive comments on my research design and implementation. Thanks to all of my classmates for their tips on my data analysis methods and their peer evaluation which helped me improve my work. Thanks for the wonderful class atmosphere!
- **Project Summary**: 
  - **Background/Motivation**
    
    Global CO2 emissions from energy combustion and industrial processes grew by 0.9% or 321 Mt in 2022, reaching up to a new all-time high of 36.8 Gt (IEA 2023). However, Emissions need to fall to 9.7 Gt in 2050 for an emissions pathway compatible with the 2 °C target of the Paris Agreement (Gielen et al. 2019). Renewable energy makes up most of the emission reductions. Therefore, with the growing global demand for renewable energy, understanding the main factors affecting energy consumption becomes crucial. The proliferation of renewable energy is essential for achieving climate targets, reducing dependence on fossil fuels, and promoting sustainable economic development.
    
  - **Research Questions**
    1. What is the current CO2 emission situation globally?
    2. Which is the best model, among linear regression, random forest, and gradient boosting, that fits the prediction curve concerning renewable energy consumption in Asia?
    3. What is the trend of renewable energy consumption in Asia going in the coming 3 years?

  - **Application Scenario (Data Source)**
    
    [Global data on sustainable energy (2021-2022)](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators) from WDI and [Global data on sustainable energy (2000-2020)](https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy) on Kaggle. A total of one dataset with 21 columns and 3649 data items is involved.
    
  - **Methodology**

    First, this research applies data visualization to uncover the CO2 Emission Situation and raises the significance of energy consumption. Second, it provides classification by continent and then continues to focus on Asia. Third, it explores the Correlation among indicators via Heatmap and Scatterplot, to find the significant features of renewable energy consumption. Last, this research applies three models for Prediction: Linear Regression, Random Forest, and Gradient Boosting; and the VAR (Vector autoregressive model) for forecasting the future trend.
    
  - **Results**

    The study found that Carbon dioxide emissions have fluctuated rapidly over the past two decades. Moreover, Asia's energy consumption is growing significantly. In addition, through the VAR model, the study finds that renewable energy consumption in Asia will continue to rise in the coming years till 2025.
    
  - **Intellectual Merits and Practical impacts of your project**

    1. Through a combination of exploratory data analysis and predictive modeling techniques, this research raises the significance of renewable energy and provides the forecasting of energy consumption trends.
    2. By leveraging this dataset, this research intends to uncover insights into the evolving landscape of energy consumption patterns. This endeavor contributes to well-informed decision-making in the domains of energy policies and investments.


## Table of Contents
- literature
- method
- data
- code
- results
- spotlight
- more about the author
- references

## Literature
The existing research uses the SVR model for forecasting energy consumption, focused on China (Meng et al., 2022). In my research, I apply the VAR model for forecasting renewable energy consumption in Asia, which covers a larger area. VAR is especially useful for forecasting interrelated time series and analyzing the dynamic impact of random disturbances, which means it can capture the relationship between several variables over time. However, the prediction accuracy of 97.5% is a bit lower than the existing research, which is possibly because of the diversity in Asian countries.
![image](DataQueryCode.png)

## Method
Folder here containing more details about The Prediction Problem and The Machine Learning Workflow

## Data
Folder here containing more details about queried data and processed data

## Code
Folder here containing more details about 

## Result
Folder here containing more details about 

## Spotlight

Folder here containing all applied figures 

## More about the Author
![Description of Image](spotlight/YimingYuan.png)

Yiming Yuan, an undergraduate at Duke Kunshan University, majored in Applied Mathematics. My interests are in mathematics, especially probability and statistics; in disciplinary learning, especially machine learning. I was a research assistant studying the impacts on mental health from climate change based on sentimental analysis; I also have experience in image recognition based on Nmist and Cifar.

## Resume

**Complete PDF version here**
[github-Yiming Yuan-Resume.pdf](https://github.com/Rising-Stars-by-Sunshine/Stats201-Yiming-ML-Project/files/13659169/github-Yiming.Yuan-Resume.pdf)


- **Final reflections** 
  - **intellectual growth**
    
  - **professional growth**
    
  - **living a purposeful life**
    

## References

### Data Source
- [Global data on sustainable energy (2021-2022)](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators) from WDI
- [Global data on sustainable energy (2000-2020)](https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy) on Kaggle
### Code Source
- [CO2 Emission](https://www.kaggle.com/code/tushal01/global-co2-emission)
- [Prediction](https://www.kaggle.com/code/patrykpiesiak/eda-predicting-consumption-trends)

### Articles
- [What the Future of Renewable Energy Looks Like](https://earth.org/the-growth-of-renewable-energy-what-does-the-future-hold/)
### Literature
- Bettarelli, Luca, Davide Furceri, Pietro Pizzuto, and Nadia Shakoor. 2023. "Environmental Policies and Innovation in Renewable Energy." International Monetary Fund. September 1. https://www.imf.org/en/Publications/WP/Issues/2023/09/01/Environmental-Policies-and-Innovation-in-Renewable-Energy-538759.
- Dolf Gielen, Francisco Boshell, Deger Saygin, Morgan D. Bazilian, Nicholas Wagner, Ricardo Gorini,The role of renewable energy in the global energy transformation,Energy Strategy Reviews, Volume 24, 2019, Pages 38-50, ISSN 2211-467X, https://doi.org/10.1016/j.esr.2019.01.006.
- IEA (2023), CO2 Emissions in 2022, IEA, Paris https://www.iea.org/reports/co2-emissions-in-2022 
- Jun Wen, Chukwuemeka Valentine Okolo, Ifeanyi Celestine Ugwuoke, Kibir Kolani,
Research on influencing factors of renewable energy, energy efficiency, on technological innovation. Does trade, investment and human capital development matter?
Energy Policy, Volume 160, 2022, 112718, ISSN 0301-4215, https://doi.org/10.1016/j.enpol.2021.112718.
- Meng, Zhaosu, Huike Sun, and Xi Wang. “Forecasting Energy Consumption Based on SVR and Markov Model: A Case Study of China.” Frontiers, April 6, 2022. https://www.frontiersin.org/articles/10.3389/fenvs.2022.883711/full. 
 



