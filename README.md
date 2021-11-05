# T3_loocv
task: given csv provided, load it in a pandas dataframe and implement leave one group out cross validation and results storing. 
note: use a RandomForestRegressor model for training with fixed random seed


use sklearn leave one group out cross validation, in the df, the group is represented by the column 'pid'.
store all the cv scores in a dictionary or list or ... for every held out group, for metrics RMSE and MAPE. -> result =  {test_pid:'1', RMSE:'3,4', Mape:'0.3'}
with the afromentioned storage***, calculate mean(RMSE) and mean(MAPE), 
If is possible, i would like to save, during cross val, training and test fold as csv, for every operation

Also, it should be verified that, when there is only one row for group, the leave one group out cross validation function in sklearn behaves in the same exact way as the leave one out cross valudation. 


*** example:
{test_pid:'1', RMSE:'1', Mape:'0.1'}

{test_pid:'2', RMSE:'2', Mape:'0.2'}

{test_pid:'3', RMSE:'3', Mape:'0.3'}

mean -> {RMSE:'2', Mape:'0.2'}

