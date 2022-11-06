# Diamond-Price-Regression 
Regression task using diamond data set to predict the diamond price, It's a great dataset for beginners learning to work with data analysis and visualization.

## About Dataset
Context
This classic dataset contains the prices and other attributes of almost 54,000 diamond
####  can  download the data from kaggle through this link: https://www.kaggle.com/competitions/shai-ml/data
### Attirbutes

- price in US dollars (\$326--\$18,823)

- carat weight of the diamond (0.2--5.01)

- cut quality of the cut (Fair, Good, Very Good, Premium, Ideal)

- color diamond colour, from J (worst) to D (best)

- clarity a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))

- x length in mm 

- y width in mm 

- z depth in mm 

- depth total depth 

- table width of top of diamond relative to widest point 

## How working with this dataset

1- recovering the data by using python libraries (Numpy, Pandas, Seaborn, Matplotlib)

    --  There is no null values

    --  There are zero values in 'x', 'y', 'z' features

2- we replace all zero values with a median value

    --  There are a lot of outliers 

3- we use log transform to remove outliers by changing data distribution to semi-normal distribution

    --  There are three categorical features 

4- we transform them into the ordinal encoder by using a manual method

5- Split the data into labels and targets,and prepare it for training

6- Training Models: we try several models { linear, SVR, KNN, XGB, Random Forest, Decision tree }

7- we calculate RMSE and Score measures for each one

8- The best result was with using XGBRegression with RMSE is 540, and a Score is 0.98

9- Get prediction using test data, and prepare a submission CSV file to submit.or each one

