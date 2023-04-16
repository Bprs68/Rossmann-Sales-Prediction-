<h1 align ='center'> Rossmann Sales Prediction </h1>
<img src="https://miro.medium.com/max/1000/0*IpUXpwNleNMgpPFr.png">

<h2>1. Problem Statement and Project Description</h2>
<p>Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.</p>

<p>In this project, we are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set. Note that some stores in the dataset were temporarily closed for refurbishment.</p>

## 2. Approach
<p>started by pre-processing and cleaning the data before moving to Exploratory Data Analysis to gain insights into our data. After understanding the data, we moved ahead to select models and applying them. We tried tuning hyperparameters to improve our model performance as well.</p>

<b>Steps involved:</b>
<ol>
  <li>Exploratory Data Analysis</li>
  <li>Manipulation and Feature Engineering</li>
  <li>Model Selection</li>
  <li>Modelling</li>
  <li>Applying Models</li>
  <li>Model Performance and Evaluation</li>
  <li>Conclusion</li>
  <li>Recommendations</li>
</ol>

## 3. Conclusion
<p>We had sales data for around 2.5 years, and we had to predict sales prices for the next six weeks. After cleaning the data, we took all the data points with some sales to split data into Test and Train data. Thereafter, we performed StandardScaling techniques to get scale data and started fitting models on it.</p>
<p>We selected the decision tree as our base model and then went ahead with the RandomForest and LGBMRegressor models. RandomForest with its parameters tuned gave us the maximum r2 score, although it was least different from the RandomForest model with default Parameters.</p>
<p>Some important conclusions drawn from the analysis are as follows:</p>
<ul>
    <li>There were more sales on Monday, probably because shops generally remain closed on Sundays, which had the lowest sales in a week. This validates the hypothesis about this feature.</li>
    <li>There is a high correlation between Customers and Sales.</li>
    <li>Stores in close proximity had more sales than those with large competition distance. This can be due to location and accessibility factors.</li>
    <li>Store type B, though being few in number, had the highest sales average. The reasons include all three kinds of assortments, especially assortment level b, which is only available at type b stores and being open on Sundays as well.</li>
    <li>Outliers were genuine in our dataset, and that's why instead of treating them, we let them be there and went with models that are not impacted by them.</li>
</ul>

## 4. Recommendations
Based on our analysis, we recommend that Rossmann should focus on the following strategies to increase their sales:
<ol>
  <li>Implement more promotional offers and discounts during weekdays, especially on Mondays.</li>
  <li>Improve accessibility and location of stores, particularly in areas with high competition distance.</li>
  <li>Increase the number of stores with assortment level b and consider opening on Sundays to increase sales.</li>
  <li>Train store managers to improve their forecasting skills and provide them with tools to predict sales accurately.</li>
</ol>

## References
<ul>
  <li>ScikitLearn Documentation</li>
  <li>MachineLearningMastery</li>
  <li>Seaborn documentation</li>
  <li>GeekForGeek</li>
  <li>AnalyticsVidhya</li>
  <li>TowardsDataScience</li>
  <li>KrishNaik</li>
  <li>AlmaBetter</li>
</ul>
