# Symptom-Based Disease Diagnosis Web App

## Overview
Welcome to the Symptom-Based Disease Diagnosis Web App project! This application leverages the power of machine learning and Flask to help users identify potential illnesses based on their reported symptoms. Our goal is to make healthcare more accessible and user-centric by providing instant and accurate predictions along with comprehensive information about each disease.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Model Training](#model-training)
- [Contributing](#contributing)
- [License](#license)

## Features
- **User-Friendly Interface:** Intuitive and easy-to-navigate interface for inputting symptoms.
- **Accurate Predictions:** Utilizes a pre-trained Decision Tree Classifier model to provide accurate disease predictions.
- **Comprehensive Information:** Provides detailed information about predicted diseases, including descriptions, precautions, medications, diet recommendations, and workout tips.
- **Educational Content:** Includes informative blog posts about various health topics to empower users with knowledge.

## Installation
Follow these steps to set up the project locally:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/symptom-diagnosis-app.git
    cd symptom-diagnosis-app
    ```

2. **Create a virtual environment:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Flask app:**
    ```bash
    flask run
    ```

## Usage
1. Open your web browser and go to `http://127.0.0.1:5000`.
2. Enter your symptoms in the provided input fields.
3. Click on the "Submit" button to get the predicted disease.
4. View the detailed information about the predicted disease.

## Model Training
The machine learning model used in this project is a Decision Tree Classifier. To train the model:

1. **Prepare the dataset:** Ensure that `symptoms_diseases.csv` is placed in the `data/` directory.
2. **Train the model:**
    ```bash
    python model/train_model.py
    ```

This will generate a `decision_tree_model.pkl` file in the `model/` directory.

## Contributing
We welcome contributions to improve this project. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Make your changes and commit them with descriptive messages.
4. Push your changes to your fork.
5. Open a pull request to the main repository.

## License
This project is licensed under the Python License. See the LICENSE file for details.

![Screenshot 2024-07-21 132258](https://github.com/user-attachments/assets/958f60b3-cbf5-40fa-83ce-a6dcb889f132)

