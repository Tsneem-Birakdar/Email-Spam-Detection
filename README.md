# Email Spam Detection using Machine Learning

## 📌 Project Overview
This project is a machine learning application that classifies email messages as **Spam** or **Not Spam**. It uses Natural Language Processing (NLP) techniques and the Multinomial Naive Bayes algorithm to analyze text messages and predict their categories.

The project also includes a simple graphical user interface (GUI) built with Tkinter, allowing users to enter a message and check whether it is spam.

## 🎯 Project Objectives
- Analyze and preprocess email message data.
- Remove duplicate records and handle missing values.
- Convert text messages into numerical features using TF-IDF.
- Train a machine learning model to classify messages.
- Evaluate model performance using accuracy and a confusion matrix.
- Build a user-friendly interface for spam detection.

## 🛠️ Technologies Used
- **Python**
- **Pandas** – Data manipulation and preprocessing.
- **NumPy** – Numerical operations.
- **Matplotlib** – Data visualization.
- **Seaborn** – Confusion matrix visualization.
- **Scikit-learn** – Machine learning and model evaluation.
- **TF-IDF Vectorizer** – Text feature extraction.
- **Multinomial Naive Bayes** – Classification algorithm.
- **Tkinter** – Graphical user interface.

## 📂 Dataset
The project uses an email dataset stored in a CSV file with the following columns:

- `Category`: The message label (`ham` or `spam`).
- `Message`: The email or text message content.

The labels are converted into numerical values:

- `ham` → `0` (Not Spam)
- `spam` → `1` (Spam)

The dataset used in this project is available on Kaggle:

[Spam Email Classification Dataset](https://www.kaggle.com/datasets/ashfakyeafi/spam-email-classification)

The dataset is used for training and evaluating the spam classification model.

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Load the dataset using Pandas.
- Explore the dataset and check its shape and information.
- Identify missing values and duplicate records.
- Remove duplicate rows and records with missing categories or messages.
- Convert message categories into numerical labels.

### 2. Exploratory Data Analysis (EDA)
Visualize the distribution of Spam and Not Spam messages using a bar chart.

### 3. Feature Extraction
Use `TfidfVectorizer` to convert text messages into numerical feature vectors that can be processed by the machine learning model.

### 4. Model Training
- Split the dataset into training and testing sets.
- Use an 80% training set and a 20% testing set.
- Train a `MultinomialNB` classifier on the transformed training data.

### 5. Model Evaluation
Evaluate the trained model using:
- **Accuracy Score** – Measures the proportion of correctly classified messages.
- **Confusion Matrix** – Shows correct and incorrect predictions for both classes.

### 6. Graphical User Interface (GUI)
The project includes a simple Tkinter application where users can:
1. Enter a message.
2. Click the **Check** button.
3. View the prediction: **Spam** or **Not Spam**.

## 📊 Model Performance
The model's accuracy is calculated on the test dataset and displayed when the program runs.

The confusion matrix is visualized using Seaborn to help analyze the classification results.

> The actual accuracy depends on the dataset and should be reported after running the model.

## 🚀 How to Run the Project

1. Install Python and Jupyter Notebook.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Open `Email Spam Detection.ipynb` in Jupyter Notebook.
4. Run all cells in order to train the model, evaluate its performance, and launch the Spam Detection GUI.

The application will train the model, display the evaluation results, and open the Spam Detection GUI.

## 📁 Project Structure
```text
Email-Spam-Detection/
│
├── email.csv
├── Email Spam Detection.ipynb
└── README.md
```

If the project is organized as a Jupyter Notebook, replace `spam_detection.py` with your notebook filename.

## 🔮 Future Improvements
- Improve classification performance through hyperparameter tuning.
- Add precision, recall, and F1-score evaluation.
- Enhance the GUI design and user experience.
- Support loading and classifying multiple messages.
- Save the trained model and TF-IDF vectorizer to avoid retraining every time.

## 👩‍💻 Author
**Tsneem Birakdar**

## 📄 License
This project is intended for educational and learning purposes.
