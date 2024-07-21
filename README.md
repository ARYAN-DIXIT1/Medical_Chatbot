<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README - Symptom-Based Disease Diagnosis Web App</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/5.3.1/css/bootstrap.min.css">
</head>
<body>
    <div class="container my-4">
        <h1>Symptom-Based Disease Diagnosis Web App</h1>

        <h2>Overview</h2>
        <p>
            Welcome to the Symptom-Based Disease Diagnosis Web App project! This application leverages the power of machine learning and Flask to help users identify potential illnesses based on their reported symptoms. Our goal is to make healthcare more accessible and user-centric by providing instant and accurate predictions along with comprehensive information about each disease.
        </p>

        <h2>Table of Contents</h2>
        <ul>
            <li><a href="#overview">Overview</a></li>
            <li><a href="#features">Features</a></li>
            <li><a href="#installation">Installation</a></li>
            <li><a href="#usage">Usage</a></li>
            <li><a href="#project-structure">Project Structure</a></li>
            <li><a href="#model-training">Model Training</a></li>
            <li><a href="#contributing">Contributing</a></li>
            <li><a href="#license">License</a></li>
        </ul>

        <h2 id="features">Features</h2>
        <ul>
            <li><strong>User-Friendly Interface:</strong> Intuitive and easy-to-navigate interface for inputting symptoms.</li>
            <li><strong>Accurate Predictions:</strong> Utilizes a pre-trained Decision Tree Classifier model to provide accurate disease predictions.</li>
            <li><strong>Comprehensive Information:</strong> Provides detailed information about predicted diseases, including descriptions, precautions, medications, diet recommendations, and workout tips.</li>
            <li><strong>Educational Content:</strong> Includes informative blog posts about various health topics to empower users with knowledge.</li>
        </ul>

        <h2 id="installation">Installation</h2>
        <p>Follow these steps to set up the project locally:</p>
        <ol>
            <li><strong>Clone the repository:</strong>
                <pre><code>git clone https://github.com/your-username/symptom-diagnosis-app.git
cd symptom-diagnosis-app
                </code></pre>
            </li>
            <li><strong>Create a virtual environment:</strong>
                <pre><code>python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
                </code></pre>
            </li>
            <li><strong>Install dependencies:</strong>
                <pre><code>pip install -r requirements.txt
                </code></pre>
            </li>
            <li><strong>Run the Flask app:</strong>
                <pre><code>flask run
                </code></pre>
            </li>
        </ol>

        <h2 id="usage">Usage</h2>
        <ol>
            <li>Open your web browser and go to <code>http://127.0.0.1:5000</code>.</li>
            <li>Enter your symptoms in the provided input fields.</li>
            <li>Click on the "Submit" button to get the predicted disease.</li>
            <li>View the detailed information about the predicted disease.</li>
        </ol>

        <h2 id="project-structure">Project Structure</h2>
        <pre><code>
symptom-diagnosis-app/
│
├── app/
│   ├── static/
│   │   ├── css/
│   │   └── js/
│   ├── templates/
│   │   ├── about.html
│   │   ├── contact.html
│   │   ├── index.html
│   │   └── blog.html
│   ├── __init__.py
│   ├── models.py
│   └── routes.py
│
├── data/
│   └── symptoms_diseases.csv
│
├── model/
│   ├── decision_tree_model.pkl
│   └── train_model.py
│
├── tests/
│   ├── test_model.py
│   └── test_routes.py
│
├── .gitignore
├── README.md
├── requirements.txt
└── run.py
        </code></pre>

        <h2 id="model-training">Model Training</h2>
        <p>
            The machine learning model used in this project is a Decision Tree Classifier. To train the model:
        </p>
        <ol>
            <li><strong>Prepare the dataset:</strong> Ensure that <code>symptoms_diseases.csv</code> is placed in the <code>data/</code> directory.</li>
            <li><strong>Train the model:</strong>
                <pre><code>python model/train_model.py
                </code></pre>
            </li>
        </ol>
        <p>This will generate a <code>decision_tree_model.pkl</code> file in the <code>model/</code> directory.</p>

        <h2 id="contributing">Contributing</h2>
        <p>
            We welcome contributions to improve this project. To contribute:
        </p>
        <ol>
            <li>Fork the repository.</li>
            <li>Create a new branch for your feature or bugfix.</li>
            <li>Make your changes and commit them with descriptive messages.</li>
            <li>Push your changes to your fork.</li>
            <li>Open a pull request to the main repository.</li>
        </ol>

        <h2 id="license">License</h2>
        <p>
            This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.
        </p>
    </div>

    <script src="https://stackpath.bootstrapcdn.com/bootstrap/5.3.1/js/bootstrap.bundle.min.js"></script>
</body>
</html>
