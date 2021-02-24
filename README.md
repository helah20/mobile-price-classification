#   [mobile-price-classification](https://www.kaggle.com/iabhishekofficial/mobile-price-classification)

##	CONTENTS :
-	Project Overview
-	Data  description
-	Notebooks
-	Applyed Models
-	The Process of work
-	compare Model score




##  Project Overview

The goal of  this project is to develop classification model for dataset that hold specifications of 2000 mobile phones attempt to predict best price ranges by applying various machine learning algorithm.

## Data  description :

* battery_power:	Total energy a battery can store in mAh 
* blue:	Has bluetooth or not	
* clock_speed:	Speed at which microprocessor executes instructions	
* dual_sim:	Has dual sim support or not	
* fc:	Front Camera mega pixels
* four_g:	Has 4G or not
* int_memory:	Internal Memory in Gigabytes
* m_dep:	Mobile Depth in cm
* mobile_wt:	Weight of mobile phone	
* n_cores:	Number of cores of processor
* pc:	Primary Camera mega pixels
* px_height:	Pixel Resolution Height
* px_width:	Pixel Resolution Width
* ram:	Random Access Memory in Megabytes
* sc_h:	Screen Height of mobile in cm
* sc_w:	Screen Width of mobile in cm	
* talk_time:	Longest time that battery will last by a call
* three_g:	Has 3G or not	
* touch_screen:	Has touch screen or not	
* wifi:	Has wifi or not


##  Notebooks:
Included in this github are a jupyter notebooks folder containing:

*   EDA_Mobile_Price_Classification.ipynb :
       - A notebook where I performed significant EDA to explore the variables.

*   Mobile_Price_Classification_ML.ipynb :
       - I began with baseline models and continued through random forest, K nearest neighbor, Decision tree , and finally  Stacking models.
	

# Applyed Models :

-  [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
-  [Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
-  [KNeighbors Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
-  [StackingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.StackingClassifier.html)


# The Process of work :
#### 1. Exploratory Data Analysis
-	find if there is duplicated and null value and clean it. 
-	visualize data and check if there is outlier. 

###### the dataset is clear from null and duplicated values and the outlier  looking normal


##	**The first thing I did was take a look at the relationship between the feature**
![image](https://github.com/helah20/mobile-price-classification/blob/main/images/heatmap.png)
<br><br>

##	**Here is the amount of each catogrical feature**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/countplot.png)

<br><br>
##	**Here we can see the amount of each catogrical feature with low cost 0**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/price_range_0.png)
<br><br>
##	**Here we can see the amount of each catogrical feature with medium cost 1**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/price_range_1.png)


<br><br>
##	**Here we can see the amount of each catogrical feature with  high cost 2**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/price_range_2.png)

<br><br>
##	**Here we can see the amount of each catogrical feature with very high cost 3**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/price_range_3.png)


##	**Here I use pie to know the amount of the phones that support  wifi , buetooth**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/wifi%2Cblue.png)

<br><br>

##	**Here I use pie to knowthe amount of the phones that support  3G , 4G**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/3G%2C4G.png)

<br><br>

##	**Here I use pie to know the amount of the phones that support  dual sim , tuoch screen**

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/dual%2C%20touch.png)

<br><br>


####	Observations:

*	we obtain that we had the sam amount of praice range over the data 
*	the data include old speicification 
*	RAM has biggest effict on price 
		*	In 0 (low cost) Ram values are changing between 0- 2000 megabytes
		*	In 1 (medium cost) Ram values are changing between 0-3000 megabytes
		*	In 2 (high cost) Ram values are changing between 1000-4000 mb
		*	In 3 (very high cost) Ram values are changing between 2000 and 4000 mb( mostly 3500-4000 mb)

 <br><br>

#### 2. Split the data to X & y for train the models.
-   X fot all feature withot price_range
-   y for target (price_range)
  <br><br>
#### 3. Defined Baseline model
- to make sure the model that we will use is appropriate for the problem
 <br><br>
#### 4. defined classification model 

-	Random forest model (rf)
-	K nearest neighbor model (knn)
-	Decision tree model (dt)
    <br><br>
#### 5. valuate model using cross validation. 
 **Why do we need cross validation in machine learning ?**
Cross-validation is primarily used to estimate the skill of a machine learning model on unseen data.That is, to use a limited sample in order to estimate how the model is expected to perform in general when used to make predictions on data not used during the training of the model.
<br><br>
#### 6. define stack model.

<p> Stacking, also known as stacked generalization, is an ensemble method where the models are combined using another machine learning algorithm </p>
<br><br>

#### 7.valuate model using cross validation. 
<br><br>

#### 8. optimize the best model using grid search. 
<p> Grid search is essentially an optimization algorithm which lets you select the best parameters for your optimization problem from a list of parameter options that you provide, hence automating the 'trial-and-error' method.</p>
<br><br>

#### 10. split the data using train_test_split from scikitlearn  and apply the best model

<br><br>
##	compare Model score 


![image](https://github.com/helah20/mobile-price-classification/blob/main/images/Model_comparsion.png)


#### 	Note :
* Random forest model (rf)
* K nearest neighbor model (knn)
* Decision tree model (dt)
* Stacking model (staked)
* Stacking model after optimizing (grid)

<br><br>
#  References :
* [kaggle](https://www.kaggle.com/)
* [8-basic-techniques-that-make-your-data-better](https://www.altexsoft.com/blog/datascience/preparing-your-dataset-for-machine-learning-8-basic-techniques-that-make-your-data-better/)
* [scikit-learn.org](https://scikit-learn.org/stable/supervised_learning.html)
* [How to Train a Final Machine Learning Model](https://machinelearningmastery.com/train-final-machine-learning-model/)
* [final-machine-learning-model](https://machinelearningmastery.com/train-final-machine-learning-model/)

