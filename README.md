# Deploy ML model with Flask to Heroku

Click the button below to quickly clone and deploy into Heroku acount.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Once deployed to your Heroku instance run the following:

```bash
curl -s -XPOST 'https://<name-of-your-heroku-app>.herokuapp.com/' -d '{"rate":5, "sales_in_first_month":200, "sales_in_second_month":400}' -H 'accept-content: application/json'
```

Alternatively a simple python script:

```python
import requests
import json
url = 'https://<name-of-your-heroku-app>.herokuapp.com/'
data = {"rate":5, "sales_in_first_month":200, "sales_in_second_month":400}
response = requests.post(url, json.dumps(data))
print(response.json())
```


## Installation

`pip install scikit-learn pandas numpy flask`

`python model.py`

`python app.py`


# Inspiration

 - **Article**: [Towards Data Science: Create an API to Deploy Machine Learning Models using Flask](https://towardsdatascience.com/create-an-api-to-deploy-machine-learning-models-using-flask-and-heroku-67a011800c50)
 - **demo** [PredictivApp](https://predictivapp.herokuapp.com/)

