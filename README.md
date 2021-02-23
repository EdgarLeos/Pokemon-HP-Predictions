# Pokemon HP Predictions

## Introduction
For our project, we worked on a Pokemon dataset that includes the type of Pokemon and their statistics. The objective of this 
project is to predict the Pokemon's HP based off of the given information. This project might be a bit challenging 
but definitely worth the struggle as we will be discovering new ways to identify a Pokemon's HP based on essential information. This project allows us 
to relive our childhood. If we are able to predict the Pokemon's HP based on the Attack, Defense, Sp. Atk, Sp. Def, Speed, and Generation we essentually become better "pokemon trainers" and eventually pokemon masters.

## Selection of Data

This project consists of the Pokemon.csv data set which includes **13 features**, with **800 samples**. The data set consists of columns pertaining to the 
Pokemon's statistics such as: Type, HP, Attack, Defense, etc. Some of the features that will be used as predictors are: _HP_, _Attack_, _Defense_, 
_Sp. Atk_, _Sp. Def_. 

After getting an idea of the data that we were working with, we decided to drop **Total** and **Type 2** as those features would not be needed 
in order to make our predictions. After dropping some features, the data that was left behind contained **2 categorical features**: _Name_, and _Type 1_ and **8 numerical features**: 
_#_, _HP_, _Attack_, _Defense_, _Sp. Atk_, _Sp. Def_, _Speed_, and _Generation_.

## Methods:
**Tools:**

- Numpy, Pandas, Matplotlib, and Seaborn for data analysis and visualization
- Scikit-learn for inference
- Github for code sharing and storing code
- Anaconda for Juypter Notebook (Converting visuals to PDF with better formatting)
- Google Colaboratory as IDE

**Inference Methods used with Scikit**
- Models: KNeighborsRegressor, LinearRegression, and PolynomialFeatures

## Results:

After scaling the data and analyzing the results, we noticed that as the HP went up, the rest of the stats went up as well except for Defense and Speed. If we stop to think about this analysis, it makes sense because the bigger the pokemon get they usually have more HP and their speed normally goes down. The same thing can be said about the defense of a bigger pokemon compared to a smaller pokemon because a smaller pokemon will have more evasiveness because of their size. 

## Discussion

After trying various regression algorithms and different models, we found that the best algorithm to use was a mixture of having the model be **KNeighborsRegressor** with the algorithm being **brute** and metric being **manhattan**. When predicting through **LinearRegression** we had **337 out of 800** pokemon not predicted correctly. Once we used the more efficient model and algorithm (KNeighborsRegressor), we were able to obtain a higher percantage of a Pokemon's HP being predicted. The predictions results that we were able to achieve were shocking to see only **9 out of 800** Pokemon were not predicted correctly.

## Summary
The Pokemon-HP-Predictions project uses a modified regression model based on 8 numerical features: #, HP, Attack, Defense, Sp. Atk, Sp. Def, Speed, and Generation. 

After running our predictions, we observed that there was an accuracy of **99.98875%** that the Pokemon's HP would be predicted correctly based on the stats of a Pokemon. That's a really high percantage being predicted correctly.
