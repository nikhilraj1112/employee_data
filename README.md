Employee Salary Prediction

 Project Description
This project aims to predict an employee's salary bracket (<= or >$50K) using a RandomForest machine learning model. It processes employee characteristics to learn patterns and make predictions. The model achieved 85.61% accuracy on the test set.

 Features
* Data Loading and Cleaning: Handles missing values ('?') by replacing them with NaN and dropping corresponding rows.
* Categorical Feature Encoding: Transforms object-type columns into numerical format using Label Encoding.
* Model Training: Utilizes a RandomForestClassifier for robust prediction.
* Model Evaluation: Provides accuracy, a detailed classification report, and a confusion matrix.
* Model Persistence: Saves the trained model and label encoders for future use.
* Visualization: Generates a confusion matrix plot for easy interpretation of model performance.

 Technologies Used
The project is developed in Python and uses the following libraries:
* `pandas` for data manipulation.
* `numpy` for numerical operations.
* `matplotlib` and `seaborn` for data visualization.
* `scikit-learn` (sklearn) for machine learning models and utilities (LabelEncoder, train_test_split, RandomForestClassifier, accuracy_score, classification_report, confusion_matrix).
* `joblib` for saving and loading Python objects, including the trained model and encoders.

 Setup and Installation

To set up and run this project locally, follow these steps:

1.  **Clone the Repository (or ensure you have the project files):**
    If you've cloned this repository from GitHub, navigate to the project directory. Otherwise, ensure all project files (`salary_prediction_model.py`, `adult 3.csv`, `Project template.pptx`, `confusion_matrix.png`, `salary_prediction_model.pkl`, `label_encoders.pkl`) are in the same folder on your local machine.

2.  **Install Python:**
    Make sure you have Python (version 3.6 or higher recommended) installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

3.  **Install Required Libraries:**
    Open your **Command Prompt** (CMD) or terminal.
    * **Recommended (Virtual Environment):** Create and activate a virtual environment to manage dependencies:
        ```bash
        python -m venv venv
        # On Windows:
        .\venv\Scripts\activate
        # On macOS/Linux:
        source venv/bin/activate
        ```
    * **Install dependencies using pip:**
        ```bash
        pip install pandas numpy matplotlib seaborn scikit-learn joblib
        ```
    * (Optional but Recommended) Generate a `requirements.txt` file:
        ```bash
        pip freeze > requirements.txt
        ```

 How to Run

1.  **Navigate to the Project Directory:**
    Open your Command Prompt (CMD) or terminal and use the `cd` command to navigate to your `project` folder (or whatever you named your project's main directory).
    Example (adjust path as needed):
    ```bash
    cd C:\Users\YourUsername\Desktop\project
    ```
    (Ensure your prompt shows the correct path, e.g., `C:\Users\YourUsername\Desktop\project>`)

2.  **Execute the Script:**
    Run the main Python script:
    ```bash
    python salary_prediction_model.py
    ```

The script will load the data, preprocess it, train the model, evaluate its performance, print the accuracy and classification report to the console, and save the model artifacts.

The following files will also be saved in your project directory:
* `salary_prediction_model.pkl`: The trained RandomForestClassifier model.
* `label_encoders.pkl`: The label encoders used for transforming categorical features.
* `confusion_matrix.png`: An image of the confusion matrix.

 Files in this Repository
* `salary_prediction_model.py`: The main Python script for salary prediction.
* `adult 3.csv`: The dataset used for training and testing the model.
* `Project template.pptx`: The presentation template for this project.
* `confusion_matrix.png`: The generated confusion matrix visualization.
* `salary_prediction_model.pkl`: The saved trained machine learning model.
* `label_encoders.pkl`: The saved label encoders.
* `README.md`: This file.
