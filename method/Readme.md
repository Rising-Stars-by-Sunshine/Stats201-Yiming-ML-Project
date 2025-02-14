In Method, I will introduce my research on Machine Learning for Prediction from the research problem and the machine learning workflow:

---

**1. The Prediction Problem**

**1.1. Research Question Formulation:** 
- **Objective:**

a. What is the current CO2 emission situation?

b. What is the best model that fits the prediction curve concerning renewable energy consumption in Asia?

c. What is the future trend of renewable energy consumption going like in Asia?

- **Significance:**
Global CO2 emissions from energy combustion and industrial processes grew by 0.9% or 321 Mt in 2022, reaching up to a new all-time high of 36.8 Gt (IEA 2023). However, Emissions need to fall to 9.7 Gt in 2050 for an emissions pathway compatible with the 2 °C target of the Paris Agreement (Gielen et al. 2019). Renewable energy makes up most of the emission reductions. Therefore, with the growing global demand for renewable energy, understanding the main factors affecting energy consumption becomes crucial. The proliferation of renewable energy is essential for achieving climate targets, reducing dependence on fossil fuels, and promoting sustainable economic development. In this research, it is significant to analyze the key factors affecting energy consumption and predict future consumption trends to provide data support for policy-making or investment decisions.

**1.2.Operational Measures:**
- **Variables:** 
I begin by selecting a target variable representing energy consumption trends, this being Primary energy consumption per capita (kWh/person), which is Y. Then, relevant features, encompassing attributes that could impact energy consumption, are X variables. They might be Renewable electricity generating capacity per capita, Low-carbon electricity (% electricity), GDP per capita, and Energy intensity level of primary energy (MJ/$2017 PPP GDP) due to their direct or indirect impact on energy utilization patterns.
Data Type: The dataset is a time series with an annual frequency.

**1.3. Hypothesis Development:**
- **Prediction Hypothesis:** 
The X variables, Renewable electricity generating capacity per capita, Low-carbon electricity (% electricity), and GDP per capita, are all positively related to the amount of renewable energy consumed. For example, Higher GDP per capita might correlate with increased energy consumption due to higher industrial and domestic energy demands. Also, policy can make great changes to energy share and consumption. What’s more, the consumption of renewable energy will increase in the future. 
 
- **Justification:** 
First of all, by common sense, we know that if citizens have easier or more access to renewable energy, consumption will increase accordingly.
Additionally, a study suggests that CCPs increase green patents from 2000 to 2021 (Bettarelli et al. 2023). This indicates that policies can indeed have a significant impact on advancing renewable energy technologies and, by extension, their share in the total energy mix.
Lastly, according to the IEA, the share of renewable energy resources is expected to reach 30% by 2024, which is a larger proportion compared to that of today (Emily 2023). It is a strong proof of my hypothesis.

- **Machine Learning Algorithm Selection:**

For the prediction part, I would like to employ three different regression models for prediction: Random Forest Regressor, Linear Regression, and Gradient Boosting Regressor. Random Forest Regressor is chosen for its ability to handle non-linear relationships, Linear Regression for simplicity and interpretability, and Gradient Boosting Regressor for its high accuracy in complex datasets (Sarswatula et al 2022). Each model has its unique strengths, which I will explore and compare, and finally find the best one to fit. 

For Forecasting the future trend, I apply the VAR model for forecasting renewable energy consumption in Asia, which covers a larger area. VAR is especially useful for forecasting interrelated time series and analyzing the dynamic impact of random disturbances, which means it can capture the relationship between several variables over time (Meng et al. 2022).

---

**2. The Machine Learning Workflow**

**2.1. Model Development:**
This dataset is a very comprehensive and completed dataset. For data processing, firstly, I plan to unify data, including column names and measurement units. Secondly, I will search for and drop rows with duplicated entries. Additionally, I will identify and address outlier values to improve data quality

**2.2. Results Presentation:**
- **Training and Testing:** 
The results will be shown by their Mean Squared Error and R-squared, in order to find the best fitted model.
The dataset is split into 80% for training and 20% for testing, which is a common splitting percentage. Model performance will be regularly evaluated during training to avoid overfitting, ensuring that the models generalize well to unseen data.

- **Data Visualization:**
First, to Visualize CO2 emissions in respective countries, I will plot line charts, bar charts, etc. Line charts will illustrate trends over time, while bar charts will compare renewable energy consumption across different regions.
Second, I may plan to do a visualized classification through region, to classify different levels of renewable energy consumption. It will make prediction work better in principle, since the data in the same group may have similar features.
Third, to showcase correlations between data embedded in the dataset, I will use the correlation heatmap, which is the most intuitive diagram.
Finally, I would try different predicting and forecasting models, including Linear Regression, Random Forest, Gradient Boosting, and VAR models, so as to predict and forecast the consumption trend in the coming three years.
 
**2.3.Model Evaluation:**
- **Evaluation Criteria:**
The results will be shown by their Mean Squared Error and R-squared, in order to find the best fitted prediction model (Sarswatula et al 2022).

- **Iterative Improvement:**

a. Ongoing Feature Evaluation:
Periodically assess the relevance of my selected features in relation to the target variable "Primary energy consumption per capita (kWh/person)." Remove or replace features that do not contribute significantly to the model's predictive accuracy.

b. Algorithm Fine-tuning: 
Optimize the hyperparameters and configurations specific to the Random Forest Regressor, Linear Regression, and Gradient Boosting Regressor.

c. Stability Assessment: 
Implement cross-validation techniques suitable for time series data to ensure stability and reliability. 

**Flowchart**
![image](method.png)

**References**
- Bettarelli, Luca, Davide Furceri, Pietro Pizzuto, and Nadia Shakoor. 2023. "Environmental Policies and Innovation in Renewable Energy." International Monetary Fund. September 1. https://www.imf.org/en/Publications/WP/Issues/2023/09/01/Environmental-Policies-and-Innovation-in-Renewable-Energy-538759.
- Dolf Gielen, Francisco Boshell, Deger Saygin, Morgan D. Bazilian, Nicholas Wagner, Ricardo Gorini,The role of renewable energy in the global energy transformation,Energy Strategy Reviews, Volume 24, 2019, Pages 38-50, ISSN 2211-467X, https://doi.org/10.1016/j.esr.2019.01.006.
- Folk, Emily. “What the Future of Renewable Energy Looks Like.” Earth.Org, April 3, 2023. https://earth.org/the-growth-of-renewable-energy-what-does-the-future-hold/.  
- IEA (2023), CO2 Emissions in 2022, IEA, Paris https://www.iea.org/reports/co2-emissions-in-2022 
- Jun Wen, Chukwuemeka Valentine Okolo, Ifeanyi Celestine Ugwuoke, Kibir Kolani,
Research on influencing factors of renewable energy, energy efficiency, on technological innovation. Does trade, investment and human capital development matter?
Energy Policy, Volume 160, 2022, 112718, ISSN 0301-4215, https://doi.org/10.1016/j.enpol.2021.112718.
- Meng, Zhaosu, Huike Sun, and Xi Wang. “Forecasting Energy Consumption Based on SVR and Markov Model: A Case Study of China.” Frontiers, April 6, 2022. https://www.frontiersin.org/articles/10.3389/fenvs.2022.883711/full.
- Sarswatula, Sai Aravind, Tanna Pugh, and Vittaldas Prabhu. “Modeling Energy Consumption Using Machine Learning.” Frontiers, May 31, 2022. https://www.frontiersin.org/articles/10.3389/fmtec.2022.855208/full.  
