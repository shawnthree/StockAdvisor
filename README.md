# StockAdvisor
StockAdvisor JupyterNotebook
# Inputting the ticker for the stock you want to predict : 
val = input("Enter your ticker: ")
# Gathering all the stock data using the ticker : 
stock_data = yf.download(tickers=val,period='5y',interval='1d')
# Plotting the stock price for about the last four years : 
plt.plot(stock_data['Open'])
# seperating the data : 
X_train, y_train = function(stock_data_train,time_stamp); X_test, y_test = function(stock_data_test,time_stamp)
# training the model : 
model.fit(X_train,y_train,validation_data=(X_test,y_test),epochs=100,batch_size=64)
# making the predictions : 
train_predict = model.predict(X_train); test_predict = model.predict(X_test)
# plotting the predictions : 
plt.plot(train_predict); plt.plot(test_predict)
