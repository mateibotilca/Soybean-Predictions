Hello! 

For this project I used a dataset about soybean cultivers from Brazil. I performed data cleaning and data processing on this dataset before completing the Exporatory Data Analysis.
EDA helped me to find details about the distribution of the MHG and GY variables as well as which are the other attributes that influence MHG and GY the most. 


I was able to respond to the following questions:

1. What are the most important factors in determining MHG (Thousand seed weight)?

  The most important factor is the season. It is the attribute from the dataset that influences the most the MHG. These two variables have a correlation of 0.31.

2. What are the most important factors in determining GY (Grain yield)?

   In this case, the most important factor is NGL with a correlation of 0.24.

3. What is the delta in MHG and GY from Season 1 to Season 2?

   The delta in MHG is 12.067 and the delta in GY is -19.797.

EDA also helped me to find the right model that I should use for predicting the MHG for a cultivar created by me.
I chose the Random Forest Regressor (Supervised learning algorithm) because of the following reasons:
a) the MHG is a cotinous value, so this was a regression problem, not a classification one;
b) the correlation between variables wasn't an excellent one so Linear Regression wasn't an option;
c) It was not such a complex dataset in order to use neural networks.

Still the Random Forest Regressor model gave me pretty big errors and low performance scores as it can be seen in the code (mean square error, mean absolute error and r2_score).
So I performed Hyper-parameter tuning and this helped me a little bit with the errors and the scores. 
Finally, I predicted the MHG for my own cultivar and the prediction was a credible one because the predicted value was similar with the values of other cultivars. 
(I gave to my own cultivar values for the input attributes that were close to the ones of other cultivars.)
   
