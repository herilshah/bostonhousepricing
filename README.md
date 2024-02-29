# Boston House Price Prediction

## Overview
This project aims to predict house prices in the Boston area using machine learning techniques. It utilizes the famous Boston Housing Dataset, which contains information about various factors affecting house prices in different neighborhoods of Boston. By training a machine learning model on this dataset, we can predict the price of a house based on its characteristics.

## Project Structure
- `app.py`: Flask application file containing the code for running the prediction API.
- `regmodel.pkl`: Pickled machine learning model trained on the Boston Housing Dataset.
- `scaling.pkl`: Pickled scaler object used to scale input features for prediction.
- `templates/`: Directory containing HTML templates for the web application.
- `static/`: Directory containing static files such as CSS and JavaScript.
- `requirements.txt`: File listing all Python dependencies required to run the project.

## Usage
1. Install the required Python packages by running:
pip install -r requirements.txt

2. Run the Flask application:
python app.py



3. Access the application in your web browser at `http://localhost:5000`.

## Input Features
The model accepts the following input features for predicting house prices:
- CRIM: Per capita crime rate by town
- ZN: Proportion of residential land zoned for lots over 25,000 sq.ft.
- INDUS: Proportion of non-retail business acres per town
- CHAS: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- NOX: Nitric oxides concentration (parts per 10 million)
- RM: Average number of rooms per dwelling
- AGE: Proportion of owner-occupied units built prior to 1940
- DIS: Weighted distances to five Boston employment centers
- RAD: Index of accessibility to radial highways
- TAX: Full-value property-tax rate per $10,000
- PTRATIO: Pupil-teacher ratio by town
- B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
- LSTAT: Percentage of lower status of the population

## Example
Here's an example of how to use the prediction API:
- Endpoint: `/predict_api`
- Method: POST
- Input: JSON object containing values for input features
- Output: Predicted house price in thousands of dollars

## Credits
- Dataset: [UCI Machine Learning Repository - Boston Housing Dataset](https://archive.ics.uci.edu/ml/datasets/Housing)
- Flask: [Flask Web Framework](https://flask.palletsprojects.com/)
- Scikit-learn: [Machine Learning Library for Python](https://scikit-learn.org/)

## License
This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
