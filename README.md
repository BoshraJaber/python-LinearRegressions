# Lab: 13 - Linear Regressions

1. split data into train data and test data
2. use train data to come up with a model
3. test the model
4. calculate accurecy 

# Solution steps:
1. import what is needed
2. read the data from the csv file and split the x and y data you want to test
3. get the value for each one
4. reshap the x data ```.reshape(-1,1)```
5. x_train, x_test, y_train, y_test = train_test_split(x,y, train_size=0.8, test_size=0.2, random_state=100)
6. build the model: ``` model = LinearRegression().fit(x_train, y_train)```
7. testing the model: ```y_predit = model.predict(x_test) ```
8. ``` print(f"Testing accuracy {model.score(x_test, y_test)*100}") ```
9. ``` print(f"Traing accuracy {model.score(x_train, y_train)*100}") ```

