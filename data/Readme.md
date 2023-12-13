## Description
This dataset is mainly queried from Kaggle (https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy), which is an open data source sorted by Ansh Tanwar. It showcases sustainable energy indicators and other useful factors across countries from 2000 to 2020. We can dive into vital aspects such as renewable energy, energy intensity, financial flows, and economic growth; and gain profound insights into global energy consumption patterns by comparisons. 

Considering the completeness and real-time nature of the data, I downloaded new data for 2021-2022 from the World Bank (https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators).

I also wrote a code to scrape data from Weibo, the data will include post texts, posting time, location, etc.. It will be applied in the causal inference part, which can indicate public feelings on policy launching.

## Sample Data

|Entity	|Year	|Access to electricity (% of population)	|Access to clean fuels for cooking|	Renewable-electricity-generating-capacity-per-capita | Financial flows to developing countries (US $)|	Renewable energy share in the total final energy consumption (%)|	Electricity from fossil fuels (TWh) | Electricity from nuclear (TWh) |	Electricity from renewables (TWh) |	Low-carbon electricity (% electricity) | Primary energy consumption per capita (kWh/person)	|Energy intensity level of primary energy (MJ/$2017 PPP GDP)|	Value co2 emissions kt by country |	Renewables (% equivalent primary energy)|	gdp_growth|	gdp_per_capita	|Density\n(P/Km2)	|Land Area(Km2)	|Latitude|	Longitude|
|--------|---------|--------|-------|---------|--------|--------|--------|--------|--------|-------|---------|--------|--------|--------|--------|--------|-------|---------|--------|--------|
| Afghanistan|	2000|	1.613591|	6.2	|9.22	|20000|	44.99	|0.16|	0	|0.31|	65.95744|	302.59482	|1.64|	760		||||		60	|652230	|33.93911	|67.709953|
|Afghanistan|	2001	|4.074574|	7.2	|8.86|	130000	|45.6|	0.09|	0	|0.5|	84.745766|	236.89185	|1.74	|730	||||			60	|652230|	33.93911	|67.709953|
|Afghanistan|	2002	|9.409158	|8.2|	8.47	|3950000|	37.83|	0.13|	0	|0.56|	81.159424	|210.86215|	1.4|	1029.999971	|	||	179.4265792|	60|	652230	|33.93911	|67.709953|
|Afghanistan|	2003|	14.738506	|9.5|	8.09|	25970000	|36.66|	0.31|	0	|0.63|	67.02128|	229.96822|	1.4|	1220.000029|	|	8.832277813	|190.6838143|	60	|652230|	33.93911	|67.709953|
|Afghanistan	|2004|	20.064968	|10.9|	7.75	||	44.24|	0.33|	0	|0.56|	62.92135	|204.23125	|1.2|	1029.999971||		1.414117981|	211.3820742|	60|	652230	|33.93911|	67.709953|

It is apparent to find that there exist null data, which should be cleaned before analysis.

## Data Dictionary for Global Data on Sustainable Energy

| Variable Name | Description | Type | Range | Units | Frequency | Additional Notes |
|--------|--------------|------|-------|---------|-----------|--------|
| Entity | The name of the country or region for which the data is reported | object | | | | eg. Afghanistan |
| Year | The year for which the data is reported | int64 | 2000 to 2020 | | annual | eg.2000 |
|Access to electricity| The percentage of population with access to electricity|float64|0-100|% of population|annual|eg. 1.613591|
|Access to clean fuels for cooking|The percentage of the population with primary reliance on clean fuels|float64|0-100 |% of population|annual|eg. 6.2|
|Renewable-electricity-generating-capacity-per-capita|Installed Renewable energy capacity per person|float64| |capacity per person|annual|eg. 9.22|
|Financial flows to developing countries |Aid and assistance from developed countries for clean energy projects|float64||US($)|annual|eg. 20000.0|
|Renewable energy share in total final energy consumption |Percentage of renewable energy in final energy consumption|float64|0-100|(%)|annual|eg. 44.99|
|Electricity from fossil fuels | Electricity generated from fossil fuels (coal, oil, gas) in terawatt-hours|float64||(TWh)|annual|eg. 0.16|
|Electricity from nuclear | Electricity generated from nuclear power in terawatt-hours|float64||(TWh)|annual|eg. 0.0|
|Electricity from renewables | Electricity generated from renewable sources (hydro, solar, wind, etc.) in terawatt-hours|float64||(TWh)|annual|eg. 0.31|
|Low-carbon electricity| Percentage of electricity from low-carbon sources (nuclear and renewables)|float64|0-100| (% electricity)|annual||
|Primary energy consumption per capita |Energy consumption per person in kilowatt-hours|float64||(kWh/person)|annual|eg. 302.59482|
|Energy intensity level of primary energy | Energy use per unit of GDP at purchasing power parity|float64||(MJ/$2011 PPP GDP)|annual|eg. 1.64|
|Value_co2_emissions | Carbon dioxide emissions per person in metric tons|float64||(metric tons per capita)|annual|eg.760.000000|
|Renewables | Equivalent primary energy that is derived from renewable sources|float64|0-100|(% equivalent primary energy)|annual|eg. 0.053235482|
|GDP growth | Annual GDP growth rate based on constant local currency|float64|0-100|(annual %)|annual|eg. 3.8|
| GDP per capita| Gross domestic product per person|float64||/capita|annual|eg. 1765.027146|
|Density| Population density in persons per square kilometer|object||(P/Km2)|annual|eg. 18|
|Land Area |Total land area in square kilometers|float64||(Km2)||eg. 2381741|
|Latitude| Latitude of the country's centroid in decimal degrees|float64||||eg. 28.033886|
|Longitude| Longitude of the country's centroid in decimal degrees|float64||||eg. 1.659626|


## flowchart
![image](DataQuery.png)
