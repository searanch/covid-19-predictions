# covid-19-predictions

This project was inspiererd by: 

This project uses machine learning to make predictions about the Covid-19 deaths in Hennepin County, Minnesota. The project uses data from the us-counties.csv and us.csv files and applies linear regression to create a model for predicting future deaths.

The code loads the county data and filters it to only include data for Hennepin County in Minnesota. It then creates a datetime object from the date field and groups the data by date. The resulting data is sorted by date and the NaN values are dropped.

The model is created using the LinearRegression class from the scikit-learn library. The model is trained on the day, month, and year features and the death count target. The data is split into training and testing sets and the model is fit to the training data.

The model is then used to make predictions for future dates, specifically Labor Day, Election Day, Thanksgiving, and Christmas. The predictions are added back to the DataFrame and graphed alongside the actual death counts.
