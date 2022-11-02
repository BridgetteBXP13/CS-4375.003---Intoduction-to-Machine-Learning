# Welcome to my Machine Learning Projects!
## Overview of Machine Learning (ML)
[Here](Overview%20of%20ML.pdf) is lovely pdf which shows a brief overview of ML.

## Data Exploration in C++
[Here](Data%20Exploration/Data%20Exploration%20in%20C%2B%2B.pdf) is a pdf about Data Exploration in C++ and the [data_exploration.cpp](Data%20Exploration/data_exploration.cpp) program. Note: It requires the [Boston.csv](Data%20Exploration/Boston.csv) input file.

## Linear Models

### Regression
In this [notebook](Linear%20Models/Regression/Regression.Rmd) we used a [Air Pollution](Linear%20Models/Regression/Air_Pollution.csv) dataset. It is also available in [pdf](Linear%20Models/Regression/Regression.pdf) form. In the notebook/pdf we did an overview of Linear Regression and created a few linear models with the air pollution dataset. First we cleaned the data set and filled in the missing values with means, then we divded the data into train and test sets. We plotted the different recorded factors. We experimented with different models, however none of them were very good at predicting one another. We believe this is because of the nature of the data and some of the data was very skewed. None the less we reviewed the summaries and explained the different metrics for judging the models. We compared the models based on the different graphs and metric values. 

### Classification
In this [notebook](Linear%20Models/Classification/Classification.Rmd) we used a [Tree Cover](Linear%20Models/Classification/covtype.csv) dataset. It is also available in [pdf](Linear%20Models/Classification/Classification.pdf) form. In the notebook/pdf we did an overview of Classification. We explored and cleaned the data, this dataset is very well done and had no empty values, it also is very large with nearly 600,000 observations. We did multiclass classification using Logistic Regression with the One vs All method. Then we used Naive Bayes Models and evaluated both. Then we evaluated the two with their metrics such as accurracy, sensitivity, specificity, kappa, ROC curves, AUC, and tried MCC but our dataset was too large and overflowed the function. Then we compared the two models and analyzed the benefits/drawbacks of the different metrics.

## Machine Learning with C++ from Scratch
In this [pdf](ML%20Algorithms%20from%20Scratch/Machine%20Learning%20with%20C%2B%2B.pdf) we do an overview of our C++ maching learning programs [Logistic Regression](ML%20Algorithms%20from%20Scratch/LogisticRegression.cpp) and [Naive Bayes](ML%20Algorithms%20from%20Scratch/NaiveBayes.cpp) from scratch. In the pdf it will go over the purpose, input, output, logic, functions, and metrics for each of our C++ machine learning logistic regression and naive bayes programs. For this we used the [titanic dataset](ML%20Algorithms%20from%20Scratch/titanic_project.csv) to classify if a person survivied or not.

### Logistic Regression

Our logistic regression model only used the 'sex' predictor and utlized vector and matrix mulitplication in C++ to perform the neccessary calculations for the logistic regression algorithm. It takes the [titanic dataset](ML%20Algorithms%20from%20Scratch/titanic_project.csv) as it's file input, if not available in the directory then it will display an error message in the terminal to the user. It will then organize the data into test/train vectors, close the file, and then create the logisitc regegression model. After that it will display the evaluation to the user showing the confusion matrix, accuracy, spensitiivty, specificity, and how long it took to create the model in microseconds. More detail can be seen in the pdf above.

### Naive Bayes

Our naive bayes model only used all the predictors except person including person's class, sex, and age and utlized vector and matrix mulitplication in C++ to perform the neccessary calculations for the naive bayes algorithm and probability calculations. Note: for age we divided it into 5 categories as follows: Kids (0-12), Teens (13-19), Adults (20-39), Mid Adults(40-59), and Seniors (60+). It takes the [titanic dataset](ML%20Algorithms%20from%20Scratch/titanic_project.csv) as it's file input, if not available in the directory then it will display an error message in the terminal to the user. It will then organize the data into test/train vectors, close the file, and then create the naive bayes model. After that it will display the evaluation to the user showing the probabilty matrix for each predictor, the predictions made overall if they survivied or not, the evaluation confusion matrix, accuracy, spensitiivty, specificity, and how long it took to create the model in microseconds. More detail can be seen in the pdf above.

## Searching for Similarity
In this project we worked in a group of four. We created four notebooks for [Regression](Searching%20for%20Similarity/Regression.pdf), [Classification](Searching%20for%20Similarity/Classification.pdf), [Clustering](Searching%20for%20Similarity/Clustering.pdf), and [Dimensionality Reduction](Searching%20for%20Similarity/Dimensionality_Reduction.pdf). Our .Rmd notebooks can be found on our github. We also wrote an [overview](Searching%20for%20Similarity/Searching%20for%20Similarity_NarrativeDoc.pdf) for all four with our findings and comparisons for each algorithm. For our regression we used the [steam](Searching%20for%20Similarity/Steam_Data/steam_amended_first_200k_players.csv.zip) database which contained statistics for the first 200k players on steam. For classification, clustering, and dimensionality reduction we used two [League of Legends](Searching%20for%20Similarity/League_Data/league_korea_high_elo_team_stats.zip) datasets which contained winning and losing team stats for the top high elo teams in the Korean server. For this dataset we predicted/classified if a team won or lost based on their stats such as kills, deaths, vision score, damage, gold earned, and crowd control for each player.


## Kernel and Ensemble
### The dataset
In this project I collaborated with Isabelle Kirby and we created three notebooks. The dataset we used was the same league of legends datasets we used in Searching for Similarity. The two [League of Legends](Kernel%20and%20Ensemble/League_Data/league_korea_high_elo_team_stats.zip) datasets which contained winning and losing team stats for the top high elo teams in the Korean server. For this dataset we predicted/classified if a team won or lost based on their stats such as kills, deaths, vision score, damage, gold earned, and crowd control for each player. However, for these models we combined each five players into 1 total stat for each category to increase speed for the models (especially for SVM). 
### SVM Kernel Notebooks
Our first notebook was for [Regression](Kernel%20and%20Ensemble%20Methods/Regression.pdf). It utilized SVM models for Linear, Polynomial, and Radial kernels. Our second notebook was for [Classification](Kernel%20and%20Ensemble%20Methods/Classification.pdf). It also utilized SVM models for Linear, Polynomial, and Radial kernels, however we had to change the 'won' column of our dataset to a factor in order to force SVM to use classification instead of regression. 
### The Ensemble
Finally our third notebook utilized Random Forest, Random Forest with Bagging, XGBoost, XGBoost with combined trees, and SuperLearner's Ranger model. Overall, all the models except ranger performed very well. I believe SuperLearner's Ranger performed poorly because we didn't spend a lot of time super tuning the parameters. We would have prefered fastAdaBoost but unfortunately it is not available in the latest R versions. We attempted AdaBag but it was taking a very very long time (even after trimming our dataset to just 27 observations!)

## ML with sklearn
In this project I practiced creating classification models for Logistic Regression, Decision Tree, and Neural Networks using python libraries pandas, seaborn, and sklearn. The [notebook](ML%20with%20skLearn/ML_with_skLearn.ipynb) contains all of my step by step code with explainations, findings, and analysis. There is also a [pdf](ML%20with%20skLearn/ML_with_skLearn.pdf) version.The data set used for this project was a very small [Auto](ML%20with%20skLearn/Auto.csv) data set containing information on cars. It only had a little under 400 observations. It's primary use was for practice and help me get familiar with pandas, seaborn, and sklearn. Overall I enjoyed this project and was refreshed getting a break from R as I have been looking forward to python and doing image classification with Tensorflow!
