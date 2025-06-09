Iris Flower Classification Web App
Overview
This is a Flask-based web application that predicts the species of an Iris flower based on user-provided measurements of sepal width, sepal height, petal width, and petal height. The application uses a Logistic Regression model trained on the Iris dataset to make predictions.
Features

Input Form: Users can input sepal width, sepal height, petal width, and petal height via a web form.
Prediction: The app predicts the Iris species (Setosa, Versicolor, or Virginica) using a trained Logistic Regression model.
Dataset: Utilizes the Iris dataset from a public GitHub repository.
Web Interface: Built with Flask and rendered using an HTML template (index.html).

Requirements
To run this project, you need the following Python packages:

Flask
NumPy
Pandas
Scikit-learn

You can install the dependencies using:
pip install flask numpy pandas scikit-learn

Project Structure

app.py: The main Flask application containing the logic for loading the dataset, training the model, and handling web requests.
templates/index.html: The HTML template for the web interface (not included in this file but required for rendering).
README.md: This file, providing an overview and instructions for the project.

How It Works

The application loads the Iris dataset from a public URL.
A Logistic Regression model is trained on the dataset's features (sepal width, sepal height, petal width, petal height) to predict the flower species.
Users access the web interface at the root URL (/), where they can input measurements.
Upon form submission, the app processes the input, makes a prediction, and displays the predicted species on the same page.

Usage

Clone the Repository:
git clone <repository-url>
cd <repository-directory>


Install Dependencies:
pip install -r requirements.txt


Run the Application:
python app.py


Access the Web App:Open a browser and navigate to http://127.0.0.1:5000.

Input Measurements:Enter the sepal width, sepal height, petal width, and petal height in the form, then submit to see the predicted Iris species.


Notes

Ensure the index.html template is present in the templates folder, as it is required for rendering the web interface.
The dataset is fetched from a public URL, so an internet connection is required.
The eval function is used to parse form inputs, which is not recommended for production due to security risks. Consider using safer alternatives like float or int for parsing in a production environment.

License
This project is licensed under the MIT License.
