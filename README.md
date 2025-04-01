This is a Flask-based web application that predicts forest fires based on given input parameters. The model is trained using machine learning techniques.

Features

User-friendly web interface

Predicts forest fire occurrence

API endpoint for programmatic access

Deployed using Flask

Machine Learning Model

The model was trained using Linear Regression, Ridge Regression, Lasso Regression, and ElasticNet. Among them, Ridge Regression was selected due to its higher accuracy.

Installation

1. Clone the Repository

git clone https://github.com/your-username/flask-forestfire.git
cd flask-forestfire

2. Create a Virtual Environment

python -m venv venv

Activate it:

Windows:

venv\Scripts\activate

Mac/Linux:

source venv/bin/activate

3. Install Dependencies

pip install -r requirements.txt

Running the Application

python app.py

The app will run on http://127.0.0.1:5000/

API Usage

Endpoint: /predict

Method: POST

Request Body (JSON example):

{
  "temperature": 30,
  "humidity": 60,
  "wind_speed": 10,
  "rain": 0.5
}

Response:

{
  "fire_risk": "High"
}

Deployment

To deploy on Heroku:

git push heroku main

Or use Render/Vercel for deployment.

License

This project is licensed under the MIT License.
