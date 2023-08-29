Rock-Paper-Scissors AI Model
Introduction

This repository contains the code for a machine learning model that simulates Rock-Paper-Scissors games against a human player. The model adapts its strategies based on the player's behavior and aims to win as often as possible. The model employs a multi-layer perceptron (MLP) neural network and is written in Python using Scikit-learn.
Features

    Various strategies for the simulated player, including 'spam', 'random', 'intelligent', and more.
    Player strategy estimation based on historical moves.
    Model adapts to win and loss streaks.
    Utilizes MLP Classifier for predictions.
    Incorporates feature scaling using Standard Scaler.
    Enables dynamic strategy adaptation through win/loss streaks and frequent moves.
    L2 regularization and early stopping to prevent overfitting.

Dependencies

    Python 3.x
    Scikit-learn
    NumPy
    Pandas
    Matplotlib
    Joblib

Install all dependencies using conda:

bash

conda install scikit-learn numpy pandas matplotlib joblib

Usage

    Clone the repository to your local machine.
    Navigate to the project directory.
    Run the rock_paper_scissors_ml.py file.
    Follow the console instructions to play the game.
    or go to the following colab and play there:
    https://colab.research.google.com/drive/1DyzDSbvt8BhytHLJpWQPgEf5_3V1yPJV?authuser=0#scrollTo=grk7rT9GYuRJ

File Structure

    rock_paper_scissors_ml.py: Main Python file containing all the code.
    DecentRPS.joblib: Serialized file for saving the trained model.
    DecentRPS_Scaler.joblib: Serialized file for saving the Standard Scaler object.

How it Works
Data Simulation

    Simulates games between the model and players using various strategies.
    Collects data on move history, win/loss streaks, and player strategies.

Data Preprocessing

    Data is shuffled and split into training and validation sets.
    Feature scaling is applied using Standard Scaler.

Model Training

    The model is trained using an MLP Classifier from scikit-learn.
    L2 regularization and early stopping are implemented to prevent overfitting.
    The model is trained for multiple epochs and evaluated on a validation set.

Real-Time Prediction

    During real gameplay, the model estimates the player's strategy and predicts the next move accordingly.
    The model adapts to the player's strategies and changes its own strategy based on win/loss streaks.

Issues and Future Work

    The model performs well, but there is room for improvement. Current plan is using the Flask script to work with Heroku on my website. Having issues there
    Potential for adding more complex strategies and features.

License

This project is open-source and available under the MIT License.
Contributing

Feel free to fork the project and submit a pull request with your changes.
Author

@nyk

For more details, feel free to check out the code and comments within. Enjoy the game!
