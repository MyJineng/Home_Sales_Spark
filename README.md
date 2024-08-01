# Home_Sales_Spark

Data on home sales was sourced from S3 and queried for statistics on price with home age, rooms, and sqr footage constraints.
The data was then cached and partitioned to evaluate which was more efficent for the query being run.

## Results

What is the average price for a four bedroom house sold per year, rounded to two decimal places?
AVG_Price_4_Bedroom: 299661.01
hat is the average price of a home for each year the home was built, that have 3 bedrooms and 3 bathrooms, rounded to two decimal places?
+----+-----------------+
|year|AVG_Price_by_Year|
+----+-----------------+
|2010|        292859.62|
|2011|        291117.47|
|2012|        293683.19|
|2013|        295962.27|
|2014|        290852.27|
|2015|         288770.3|
|2016|        290555.07|
|2017|        292676.79|
+----+-----------------+
What is the average price of a home for each year the home was built, that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet, rounded to two decimal places?
+----+-----------------+
|year|AVG_Price_by_Year|
+----+-----------------+
|2010|        285010.22|
|2011|        276553.81|
|2012|        307539.97|
|2013|        303676.79|
|2014|        298264.72|
|2015|        297609.97|
|2016|         293965.1|
|2017|        280317.58|
+----+-----------------+
What is the average price of a home per "view" rating, rounded to two decimal places, having an average home price greater than or equal to $350,000?
+----+------------------+
|view|AVG_Price_by_Views|
+----+------------------+
|  99|        1061201.42|
|  98|        1053739.33|
|  97|        1129040.15|
|  96|        1017815.92|
|  95|         1054325.6|
|  94|         1033536.2|
|  93|        1026006.06|
|  92|         970402.55|
|  91|        1137372.73|
|  90|        1062654.16|
