# First-Task
   1. I have load the csv dataset using pandas. 
   2. Checked if there is any null values are present or not. 'Age' column has 187 null values, 'Cabin' column has 687 null values and 'Embarked' Section has 2 null values.

   3. Then I have calculate the median age of all the ages present in the 'Age' column and fill all the null values of 'Age' column with the median value.

   4. In our dataset, to train a model, we dont need 'Cabin','Name','Ticket','PassengerId', these columns. So we dropped these columns.

   5. There are two categorical features i.e. 'Sex' and 'Embarked', So The categorical features are converted into Numerical values using one Hot Encoding.

   6. Now we have all the required columns.

   7. Now we have to scale the data. The 'Age' and 'Fare' section should be scaled.  So using 'StandardScaler' of Sklearn, We standardize the values of these two columns.

   8. Now we have plotted The BOX PLOT for 'Age' and 'Fair' columns only because The outliers can be found only in these two columns. So we have to remove those outliers.

   9. The IQR is a measure of statistical spread:
   Q1 (25th percentile): 25% of data falls below this value.
   Q3 (75th percentile): 75% of data falls below this value.
   IQR = Q3 - Q1
   IQR represents the middle 50% of data — from Q1 to Q3

   The upper bound = Q1 - 1.5  * IQR
   The lower bound = Q3 + 1.5 * IQR

   We will only keep those values which are in between The upper bound and The lower bound. And rest of the values are outliers.

   10. The final result is then plotted using BOX PLOT.
