# RandomForests_coefficients
A method which extracts from the RandomForest model the "coefficient" for each feature. i.e. to better understand whether a specific feature is mostly contributing positively ot negatively to the outcome.
The moethod samples obsrvations and then, calculates the difference of the mean outcome - before and after the split, for the 2 children : '<=' and the '>'.
Finally, it averages the differences for each feature and subtracts '<=' from '>' in order to get the general direction and it's intensity.
