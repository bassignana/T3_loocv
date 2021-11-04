# T3_loocv
task: given csv provided, load it in a pandas dataframe and implement leave one group out cross validation and results storing. 
note: use a RandomForestRegressor model for training with fixed random seed


use sklearn leave one group out cross validation, in the df, the group is represented by the column 'pid'.
store all the cv scores in a dictionary or list or ... for every held out group, for metrics RMSE and MAPE. -> result =  {test_pid:'1', RMSE:'3,4', Mape:'0.3'}
with the afromentioned storage***, calculate mean(RMSE) and mean(MAPE), 


*** example:
{test_pid:'1', RMSE:'1', Mape:'0.1'}

{test_pid:'2', RMSE:'2', Mape:'0.2'}

{test_pid:'3', RMSE:'3', Mape:'0.3'}

mean -> {RMSE:'2', Mape:'0.2'}

this should be all packaged in a function that takes the df as input and gives the mean result as output.

