# w207-forestcover
###Kaggle competition to predict forest cover type
https://www.kaggle.com/c/forest-cover-type-prediction

**Due Dates**

March 30<br/>Download the data and figure out how to import it into python/numpy objects so you can process it with SK­Learn. Split the data you get into training and development for running your own experiments. Establish a baseline and submit to Kaggle for verification. For your submission, you should probably train your model on all the data you have.

Random numbers scored slightly better than expected! But the results are bad, so we have a lot of room to improve.
>Your submission scored 0.14319, which is not an improvement of your best score. Keep trying!

####Feature engineering ideas:
1) Try to smooth features by coming up with a measure of distance or adjacency between plots.<br/>
2) Adjust the vertical distance to hydrology measure by the elevation. Combine vertical and horizontal distances to single measure. [Alexander Guschin][link1]

#####Most important features (determined from logistic regression coefficients)
These features are probably the most important to look at for feature engineering ideas.<br/>
 - Hillshade_3pm
 - Hillshade_9am
 - Hillshade_Noon
 - Elevation
 - Soil_Type36
 - Soil_Type9
 - Soil_Type28
 - Soil_Type27
 - Wilderness_Area4
 - Soil_Type8
 - Soil_Type25
 - Soil_Type12
 - Vertical_Distance_To_Hydrology
 - Slope
 - Horizontal_Distance_To_Fire_Points
 - Horizontal_Distance_To_Hydrology
 - Soil_Type40
 - Wilderness_Area1
 - Soil_Type37
 - Soil_Type29
 - Soil_Type30
 - Wilderness_Area2
 - Soil_Type26
 - Soil_Type22
 - Wilderness_Area3

####Other tasks:
 - [x] Standardize features
 - [ ] Identify and impute missing data
 - [ ] Grid search over the various classifiers
 - [ ] Look at implementing a kD-tree
 - [ ] Cross-validation
 


[link1]: http://nsbviewer.ipython.org/github/aguschin/kaggle/blob/master/forestCoverType_featuresEngineering.ipynb
