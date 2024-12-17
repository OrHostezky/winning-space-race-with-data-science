# Winning Space Race with Data Science
An end-to-end data science project, completed as a the capstone project for the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science) program ([course 10](https://www.coursera.org/learn/applied-data-science-capstone?specialization=ibm-data-science)), including code notebooks, a dashboard application, and a [summary presentation](Winning_Space_Race_with_Data_Science.pdf).


## Introduction

### Context:
- **SpaceX** brings an innovative ability to reuse the 1st stage of its Falcon 9 rocket, which lowers launch price by \~70% (\~$100M per launch).
- Determining 1st-stage landing outcome enables us to determine launch cost.
- Our goal is to implement a workflow to predict 1st-stage landing outcome.

### Key Questions:
- Which factors affect 1st-stage landing outcome and in what way?
- What is the rate of successful landings over time?
- Which learning algorithm performs best in this problem?


## Methodology

- Data Collection via REST-API ([notebook](Code/1__Data_Collection__API.ipynb)) and web scraping ([notebook](Code/2__Data_Collection__Webscraping.ipynb)).
- Data Wrangling ([notebook](Code/3__Data_Wrangling.ipynb)).
- Exploratory Data Analysis (EDA) via data visualization ([notebook](Code/4__EDA_DataViz.ipynb)) and SQL ([notebook](Code/5__EDA_SQL.ipynb)).
- Interactive Map using Folium ([notebook](Code/6__VizAnalytics_Folium.ipynb)).
- Dashboard Building using Plotly Dash ([script](Code/7__spacex_dash_app.py)).
- Predictive Analysis (Classification) ([notebook](Code/8__Predictive_Analysis.ipynb)).

For a detailed account of the methodology, see [summary presentation](Winning_Space_Race_with_Data_Science.pdf).


## Results

See [summary presentation](Winning_Space_Race_with_Data_Science.pdf).


## Conclusions

- **Not all data is relevant** for the problem – only some features affect success rate.
- Launches with **large payloads** generally have **higher success** rates.
- **ES-L1**, **SSO**, **HEO**, **GEO**, and **VLEO** orbits all have **very high success** rates.
- General **success** rate shows a clear trend of **increase over time**.
- **KSC LC-39A** launch site has the **highest success** rate.
- **Launch sites** are located **in proximity** to the **coast** and **equator**.
- All models performed equally well, yet the **Decision Tree model** was slightly more **generalizable** for this problem.

### Limitations and Future Work:
- **Collection of more data** is needed for model-performance evaluation of generalizability on unseen data.
- Additional **feature engineering** may improve our model efficiency and performance.
- **Ensemble methods** like Random Forest and boosting were not used, yet it is highly likely they can be wielded to improve model performance.
