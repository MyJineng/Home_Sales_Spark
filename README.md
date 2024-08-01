# Home_Sales_Spark

Data on home sales was sourced from S3 and queried for statistics on price with home age, rooms, and sqr footage constraints.
The data was then cached and partitioned to evaluate which was more efficent for the query being run.

## Results

What is the average price for a four bedroom house sold per year, rounded to two decimal places?
AVG_Price_4_Bedroom: 299661.01

What is the average price of a home for each year the home was built, that have 3 bedrooms and 3 bathrooms, rounded to two decimal places?

![image](https://github.com/user-attachments/assets/e4599e01-491e-4cb6-b4d1-0bb5979d4f8f)

What is the average price of a home for each year the home was built, that have 3 bedrooms, 3 bathrooms, with two floors, and are greater than or equal to 2,000 square feet, rounded to two decimal places?

![image](https://github.com/user-attachments/assets/7e9cd269-875a-40c5-afdb-7857cd5beaf9)

What is the average price of a home per "view" rating, rounded to two decimal places, having an average home price greater than or equal to $350,000?

![image](https://github.com/user-attachments/assets/959c52d5-3fdc-48fb-b823-f58c74cc8fc4)

The cached format was faster than partioning by views.
