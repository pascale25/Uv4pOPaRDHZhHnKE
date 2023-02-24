# Happy Customers survey

To predict customer satisfaction, supervised machine learning classification algorithms were developed. Despite no clear patterns among features being identified in the exploratory data analysis, we discovered that we needed to pay attention to the "Content_as_expected" feature due to its low score. "Delivered_on_time" and "App_ease" tended to receive the highest scores from clients.

The chi-squared test indicated that the null hypothesis was accepted in all features except "Delivered_on_time," where it was rejected. Therefore, customer satisfaction is independent of all variables except the "Delivered_on_time" variable.

New features were created, including the mean of all scores, the sum of all scores, and the percentage of overall scores. The dataset was balanced using the SMOTE technique, resulting in a dataset size of (69, 69). Eight models were tested, and the best performing model was XGBoost with an accuracy of 0.74 and AUC of 0.77.

The feature of importance analysis revealed that the most crucial feature was the "Percentage of overall scores," followed by "Contents_as_expected" score 3, "Found_everything" score 3, and "Good_price" score 4.
