# AI Camp Data Science Advanced Walkthrough
A case study put together by instructor Cameron Jackson. Note that this is an advanced version of this project that specifically uses a messy and hard-to-use dataset to give a thorough review of several of the potential work required while cleaning, exploring, visualizing, and performing machine learning during this project. It is not required for instructors to use this as a resource, but we do recommend reading through and running these notebooks to understand the story told by this data.

#### NOTE: This a very advanced example of the project in which, it is acceptable and expected for students and instructors to do a much simpler version of the project.


## 🧼 Cleaning the Data
To see just how different and dirty real world data can be, look through section 1 and section 2 of the notebook: [https://github.com/organization-x/DS-Course/blob/main/DS_Merged_Data_Exploration.ipynb](https://github.com/organization-x/DS-Course/blob/main/DS_Merged_Data_Exploration.ipynb) 
To summarize how messy the above data is, the different datasets that we were merging had several problems that I’ll list below:

1. Different Naming conventions between datasets, ie using “&” vs writing out “and”
2. Random extra spacing in the different names of countries
3. Using outdated names of countries, requiring looking up countries histories to figure out what the datasets were referring to
4. Including or excluding certain territories without any noticeable pattern
5. Missing data in certain columns

We will be using the pandas python library to manage all of our data needs throughout our project so I recommend becoming familiar with the library. At this point, you should start looking for different pieces of data that you can use to answer the question you started with. You should start to map out correlations between different pieces of information you have gathered to see if it is relevant to the thesis that you created at the beginning. You can use pandas to show a correlation map between different columns of the data to help start this conversation.

## 📠 Choosing your ML model / Training the model

To select a machine learning model, you should be very intentional in defining the thesis you are trying to prove / disapprove, then training the model accordingly based on the type of machine learning problem your thesis presents (classication or regression). 

From there, you need to be ready to use evaluation metrics and visualizations as a part of your analysis. In order to do so, we will need to split our data into train/test categories using [sklearn’s `train_test_split()` function](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html).

Here is a list of possible ML models that you can look to a guidance as you start to explore the different schools of thinking that produce different models. 

1. [SVM](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)
2. [KNN](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
3. [Neural Networks (tensorflow)](https://www.tensorflow.org/datasets/keras_example)
4. [Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
5. [Xgboost](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html)
6. [Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
7. [Naive Bayes](https://scikit-learn.org/stable/modules/naive_bayes.html)

To read up how to use a model, select the walkthrough notebook that corresponds to your model. 
