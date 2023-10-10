# Crop-Mapping
Submission for Zindi GEO-AI Challenge by ITU.


The CropLand_Data file is for data generation. I used common Sentinel 1 and Sentinel 2 features, which are named as in literature. I once used the difference between the 90th and 10th percentile of those features over a time period of 1 year to see if there are big changes ( due to harvesting f.e ). I also used the average value of those features over the period of interest. 

For the model I used different Classifiers (xgboost, catboost and lgbm ) with a random grid search. Where I trained each classifiers oncve on a specific region and once with all data. Than I used teh average of those Classifiers for my final prediction. I didn't have time to optimize the set of features for each region but I think the model can still be optimized quiet a bit. Also I think that it would also be interesting to use the standard deviation instead of the difference of percentiles. 
