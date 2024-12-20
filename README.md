# ML_Churn_Prediction
Machine Learning Customer Prediction Project
![Customer Churn](https://github.com/Genixira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/customer%20churn.png)


## 🔴 What is Customer Churning ?

![Customer Retention](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco1.JPG)

## 🔴 What are the different Churn Scenarios ?

![Churn Scenarios](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco2.JPG)

## 🔴 Decision Cycle of a Subscriber ?

![Decision Cycle](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco3.JPG)

## 🔴 What are the different Churn Segments ?

![Churn Segments](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco4.JPG)

## 🔴 Solution Overview

![Solution](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco5.JPG)


In this repository, I have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them wisely to create a model, and lately, have deployed the model.

### 🟢 For EDA, please refer to : Churn Analysis - EDA.ipynb
### 🟢 For Model Building, please refer to: Churn Analysis - Model Building.ipynb
### 🟢 For Model Deployment, please refer to app.py


### 🔵 Creating the flask API

```
app = Flask("__name__")
```

The loadPage method calls our home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
The run() method of Flask class runs the application on the local development server.
```
app.run()
```


Yay, our model is ready, let’s test our bot.
The above given Python script is executed from Python shell.

Go to Anaconda Prompt, and run the below query.
```
python app.py
```


Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


HERE'S HOW OUR FRONTEND LOOKS LIKE:

![Customer Retention](https://github.com/GeniXira/ML_Churn_Prediction/blob/main/MLProject-ChurnPrediction%20main%20images/Telco6.JPG)
