# Smart Air Pressure System Diagnostics System for Scania Truck


We applied different weights to loss function to minimize cost of service. Overall, we found the best threshold to achieve minimum cost of service at 15600 on the test set. We also validate our algorithm using K fold cross validation to evaluate robustness of our models. Overall, we are comfortable with our algorithm.
Steps for the implementation:

1. Integrated data from multiple AWS SQL tables.

2. Impute missing values using 0 and grouped mean for train data set.

3. Feature engineering of histogram information to the distance to centroids of both classes for 7 attributes, which effectively reduce 70 bin features variables to 14 distance variables.

4. Time to event analysis using histogram information.

5. Given the imbalanced nature of our sample data, we applied weighted logistic classification algorithm with feature engineering of histogram information. We effectively achieved lower run time and minimum cost of service of 15600.

6. Overall, we achieved reasonable cost of service on both training and test set.
