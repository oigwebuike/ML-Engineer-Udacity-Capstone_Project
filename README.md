# ML_Engineer_Capstone_Project

The challenge in trading predicting models is usually in the quickly varying values, which must be studied with temporal sequence as with most time-series predictions. Such models require special algorithms, because the conventional algorithms like linear regression, would not be able to take care of the presence of outliers or seasonal sporadic changes in trend. 
Here -in this project- the aim is to make as accurate as possible ‘tomorrow’s’ market price (financial outcome) from how the trend has been for a period of about 5-6 years, taking into consideration the market price of each day. This might sound a bit straight forward, however, when we compare it to predictions like value of house prices based on certain features, which uses a linear regression approach to predict the most likely outcome, given some feature values, we find out that such approach with a varying “unpredictable” event might not yield desired outcomes. This is largely because unlike the house prices, which depends on known contributing factors, stock market prices (just like weather changes) can’t be predicted as linear, because they are not based on ‘known’ features or factors.
There are a lot of factors affecting how a market price might go up (or down), sometimes these factors might be speculated, other times it might be as a result of chain of events, and such variations are usually not what conventional algorithms are built on.
I sourced my data from Yahoo, taking data of stock market prices from five major stocks viz: Google, Apple Inc, Oracle, SPY, and IBM. Dating from January 1st 2008 (2008.01.01), to December 31st   2020 (2020.12.31), a period of ten (13) years. Using the Adjacent Close (Adj Close) column of this data, my aim was to build and train a model that would learn from these data and make close predictions of future outcomes.
For such a task, special algorithms or approach is needed. I considered a few, which includes using an Artificial Neural network (an RNN or LSTM), which makes use of recursive training, where a prediction not only depends on its immediate past, but also far into the past, a model can learn, and such learning is fed back into the system for better future outcomes.
However, after various searches and tutorials, and with the new knowledge and skill I learnt using AWS, I decided to try two dynamic and powerful algorithms, the AWS in-built XGBoost (eXtreme Gradient Boosting) and the external FbProphet. These algorithms perform great because of verse performance with various distributions, datatypes and their results with variety of machine learning problems.
The best approach would be to use these algorithms and compare their outputs (predicted values) with the test data, and against a known benchmark, and the run diagnosis to calculate for RMSE, and further testing for measure of performance. R2 can also be calculated; R-squared (R2), which is the proportion of variation in the outcome that is explained by the predictor variables. In multiple regression models, R2 corresponds to the squared correlation between the observed outcome values and the predicted values by the model. The Higher the R-squared, the better the mode
The best approach is to build a model using one of the known algorithms, split the data into train and test groups, and train this model with the input train-group data, and then use the model to make predictions, and compare these predictions with the test data.
