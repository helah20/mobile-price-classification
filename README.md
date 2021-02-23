# [mobile-price-classification](https://www.kaggle.com/iabhishekofficial/mobile-price-classification):

In this project, we obtain  to explore and analyze a dataset that hold specifications of 2000 mobile phones as well as attempt to predict best price ranges for a list of mobile phones in the market by applying various machine learning algorithm.

# Data  description :

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

# Applyed Models :

-  [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
-  [Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
-  [KNeighbors Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
-  [StackingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.StackingClassifier.html)


# The Process
## 1.	Exploratory Data Analysis
    -	find if there is duplicated and null value and clean it. 
    -	visualize data and check if there is outlier. 

#### the dataset is clear from null and duplicated values and the outlier  looking normal

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/heatmap.png)

![image](https://github.com/helah20/mobile-price-classification/blob/main/images/countplot.png)



## 2.	Split the data to X & y for train the models.
## 3.	Defined Baseline model
## 4.	defined classification model 
    -	Random forest model (rf)
    -	K nearest neighbor model (knn)
    -	Decision tree model (dt)
## 5.	evaluate model using RepeatedStratifiedKFold
## 6.	validate models using cross validation. 
## 7.	define stack model.
## 8.	repeat 5 & 6 with stack model.
## 9.	optimize the best model using grid search. 
## 10.	split the data using train_test_split from scikitlearn  and apply the best model


## compare Model score 


![image](https://github.com/helah20/mobile-price-classification/blob/main/images/Model_comparsion.png)


#### Note :
* Random forest model (rf)
* K nearest neighbor model (knn)
* Decision tree model (dt)
* Stacking model (staked)
* Stacking model after optimizing (grid)



