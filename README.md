# w207-forestcover
###Kaggle competition to predict forest cover type
https://www.kaggle.com/c/forest-cover-type-prediction

**Due Dates**

March 30<br/>Download the data and figure out how to import it into python/numpy objects so you can process it with SK­Learn. Split the data you get into training and development for running your own experiments. Establish a baseline and submit to Kaggle for verification. For your submission, you should probably train your model on all the data you have.

Random numbers scored slightly better than expected! But the results are bad, so we have a lot of room to improve.
>Your submission scored 0.14319, which is not an improvement of your best score. Keep trying!

####Feature engineering ideas:
1. Try to smooth features by coming up with a measure of distance or adjacency between plots.<br/>
2. Adjust the vertical distance to hydrology measure by the elevation. Combine vertical and horizontal distances to single measure. [Alexander Guschin][link1]
3. Add in higher order terms for distances
4. Effect on temperature, sunlight of northernly facing slope amplified by slope of face. [Wikipedia][link2]

#####Most important features (determined from logistic regression coefficients)
These features are probably the most important to look at for feature engineering ideas. Determined by looking at importance in decision tree classifier.<br/>
 - 0.2275 Elevation
 - 0.1718 Wilderness_Area4
 - 0.1062 Horizontal_Distance_To_Hydrology
 - 0.0933 Horizontal_Distance_To_Fire_Points
 - 0.0906 Horizontal_Distance_To_Roadways
 - 0.0612 Soil_Type3
 - 0.0444 Vertical_Distance_To_Hydrology
 - 0.0366 Hillshade_9am
 - 0.0293 Hillshade_Noon
 - 0.0258 Aspect
 - 0.0228 Hillshade_3pm
 - 0.0140 Slope
 - 0.0106 Soil_Type12
 - 0.0091 Soil_Type29
 - 0.0078 Wilderness_Area1
 - 0.0074 Soil_Type10
 - 0.0064 Wilderness_Area3
 - 0.0052 Soil_Type2

####Other tasks:
 - [x] Standardize features
 - [ ] Identify and impute missing data
 - [x] Grid search over the various classifiers
 - [ ] Look at implementing a kD-tree
 - [ ] Cross-validation
 


[link1]: http://nbviewer.ipython.org/github/aguschin/kaggle/blob/master/forestCoverType_featuresEngineering.ipynb
[link2]: http://en.wikipedia.org/wiki/Aspect_(geography)
