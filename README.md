# Concrete Strength Prediction

This project is a machine learning web application that predicts the compressive strength of concrete based on its composition and age.

## Overview

The strength of concrete depends heavily on the ingredients used in its mixture. This application allows users to input the quantities of various mix components and uses a trained machine learning model to estimate the resulting concrete strength.

The project is divided into two primary parts:
1. **Machine Learning Model**: A Jupyter Notebook detailing the data exploration and model training process.
2. **Web Application**: A Flask interface that accepts user input and serves predictions using the saved model.

## Features

* Simple web-based user interface for data entry.
* Prediction algorithm based on eight parameters: Cement, Blast Furnace Slag, Fly Ash, Water, Superplasticizer, Coarse Aggregate, Fine Aggregate, and Age (in days).

## Getting Started

### Prerequisites

Ensure you have Python installed on your system. You will also need the following libraries:
* Flask
* numpy
* pandas
* scikit-learn

### Installation

1. Clone this repository to your local machine.
2. Install the required dependencies:
   ```bash
   pip install flask numpy pandas scikit-learn
   ```
3. Verify that the `model.pkl` file exists in the project root. If it is not present, open and run the provided Jupyter Notebook to train the model and generate the file.

### Usage

1. Open a terminal in the project directory.
2. Run the web application:
   ```bash
   python app.py
   ```
3. Open a web browser and navigate to `http://127.0.0.1:5000/`.
4. Input the concrete ingredient values and submit the form to view the predicted strength.

## Project Files

* `app.py`: The backend web server built with Flask.
* `index.html`: The frontend HTML template styled with Bootstrap.
* `concrete strength prediction machine learning model.ipynb`: The notebook used for data analysis, preprocessing, and model training.
