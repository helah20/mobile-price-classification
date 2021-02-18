# [mobile-price-classification](https://www.kaggle.com/iabhishekofficial/mobile-price-classification):

Bob has started his own mobile company. He wants to give tough fight to big companies like Apple,Samsung etc.

He does not know how to **estimate** price of mobiles his company creates. In this competitive mobile phone market you cannot simply assume things. To solve this problem he collects sales data of mobile phones of various companies.

Bob wants to find out some relation between features of a mobile phone(eg:- RAM,Internal Memory etc) and its selling price. But he is not so good at Machine Learning. So he needs our help to solve this problem.

In this problem we do not have to predict actual price but a price range indicating how high the price is.


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


# EDA :
[!image]()
[!image]()






# Applyed Models :

- [Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
-[ Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
-  [KNeighbors Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
-  [StackingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.StackingClassifier.html)






