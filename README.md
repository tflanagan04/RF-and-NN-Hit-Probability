# RF-and-NN-Hit-Probability
Two random forest models (with an extra example one) and two neural networks predicting hit probability based on pybaseball statcast features.
The first two models collect complete subsets of features while the second uses numeric and categorical imputation methods to expand the sample size.
Date range is the 2025 MLB regular season.

# Source 
Statcast data from pybaseball. This has in-depth MLB data from 2015 to present day. There is no link, it is built into Python
Import statement -----> from pybaseball import statcast

# Description
Hundreds of thousands of batted ball events in the 10+ years the library runs
118 total features 
Target variable: hit probability (1/0) 

# Features Used
11 features hand picked based on personal prediction on how they would affect hit probability
3 out of the 11 are categorical, so pd.get_dummies was used to classify each possibility into its own 1/0 column
Took the total features up to 28 in initial model

# Models Used
Random Forest
Neural Network

# Instructions
Go through each code block one by one. If you go back and try and run previous model blocks it may mess up the current ones or ones in the future.
It's best if you go from top to bottom one cell at a time.

# Insights
The neural networks outperformed the random forests overall. They had higher accuracy with faster runtime. The models without imputations slightly outperformed the ones with imputations. You'll see these results further when you run the file.

# Recommendations
For scouting or player evaluation, the three features that were consistently in the most important were launch angle, hit location, and hit distance. So, when looking at potential prospects, seeing whose success is more weighted on those three factors would in theory make them more projectible with a higher probability of success.

# Final README Note
Now your good to go with the file. I hope you enjoy the ouputs and insights!
