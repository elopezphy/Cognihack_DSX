<html>
<table style="border: none" align="left">
<tr style="border: none">
<th style="border: none"><img src="http://i.imgur.com/o1X3CAd.jpg" alt="Icon" align="left"></th>
</tr>
   <tr style="border: none">
      <th style="border: none"><font face="verdana" size="6" color="black"><b>Cognihack Data Science Track</b></font></th>
   </tr>
   <tr style="border: none">
      <th style="border: none"><font face="verdana" size="5" color="black"><b>Predicting repeat shopping likelihood with Python, Spark and Watson Machine Learning</b></font></th>
   </tr>
   <tr style="border: none">
       <th style="border: none"><img src="https://kaggle2.blob.core.windows.net/competitions/kaggle/3897/media/shoppers_lores.png" alt="Icon" align="left"> </th>
   </tr>
</table>
</html>

Our exercise will take you through the process of creating a predictive model in Python using the data manipulation and machine learning libraries distributed with Spark.  

Once we've worked through the process of reading, understanding and preparing our data and have built a simple model together, we'll deploy it to the [Watson Machine Learning service](https://datascience.ibm.com/features#machinelearning) and make it available as a real-time scoring service.  

You should spend the remaining time working as a group to speculate on how you might improve these predictions. The cognihack tutors will endeavour to assist with any experimentation to help you create and evaluate refinements to the baseline model.

# Learning goals

The learning goals of this exercise are:

-  Loading CSV files into an Apache® Spark DataFrame.
-  Exploring the data using the features within:  
    a) Spark's data wrangling Python API: __pyspark.sql__;  
    b) the __pandas__ data wrangling library; and  
    c) __matplotlib__ for exploratory plots.  
-  Engineering some basic predictive features, again using __pyspark.sql__ and Spark __user defined functions (UDFs)__.
-  Preparing the data for training and evaluation.
-  Creating an Apache® Spark machine learning pipeline.
-  Training and evaluating a model.
-  Persisting a pipeline and model in Watson Machine Learning repository.
-  Deploying the model for online scoring using Wastson Machine Learning API.
-  Scoring sample scoring data using the Watson Machine Learning API.


# Setup
Before we begin working through this notebook, you must perform the following setup tasks:

-  Sign up for the IBM Data Science Experience (using w3 credentials) and create a new project;
-  Retrieve the **Acquire Valued Shoppers Challenge** data from the [Cognihack Box folder](https://ibm.ent.box.com/folder/25592156534);
-  Import the data (in csv format) into the Data Science Experience as a 'data asset' (the transactions_subset.csv file will require decompression prior to upload);
-  Create a new notebook, using the 'import from URL' option. Use the following URL: https://github.ibm.com/Stuart-Lynn/cognihack_dsx/edit/master/cognihack_datascience_participant.ipynb
-  Make sure the notebook is configured to use a Spark 2.0 kernel and Python 2.x; and
-  Create a [Watson Machine Learning Service](https://console.ng.bluemix.net/catalog/services/ibm-watson-machine-learning/) instance (a free plan is offered).
