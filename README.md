**🤖 AutoSortAI — Intelligent Customer Support Intent Classifier**

AutoSortAI is a machine learning-based intent classification system designed to enhance customer support automation. It classifies user queries and provides relevant, predefined responses. Built with scikit-learn and Google Colab, the system uses logistic regression and TF-IDF to power fast, accurate inference.

**Project Structure**

* classifier.ipynb              \# Model training, evaluation, and prediction functions  
* main.ipynb                    \# Inference pipeline and user interaction interface  
* db.ipynb                        \# Simple in-memory user history tracking  
* intent\_classifier.pkl       \# Serialized model and label encoder  
* predictions.csv             \# Saved model predictions on test set  
* Bitext\_\*.csv                  \# Training, validation, and testing datasets

**Features**

* Intent classification using TF-IDF \+ Logistic Regression  
* Multi-class classification with over 20+ customer service intents  
* Inference interface for real-time query prediction  
* Evaluation with precision, recall, F1 score, and confusion matrix  
* User interaction history logging with timestamps  
* Model persistence via \`joblib\`

**Model Results**

* Test Accuracy: 99.39%  
* Validation F1-Score: \~ 1.00

**Requirements**

* Python 3.7+  
* pandas  
* scikit-learn  
* seaborn  
* matplotlib  
* joblib  
* Google Colab

**Dataset**  
The dataset used is a labeled customer service dataset with utterances and corresponding intents. It is divided into:

* Bitext\_Sample\_Customer\_Service\_Training\_Dataset.csv  
* Bitext\_Sample\_Customer\_Service\_Validation\_Dataset.csv  
* Bitext\_Sample\_Customer\_Service\_Testing\_Dataset.csv

**Future Improvements**

* Integrate with real-time APIs or chatbots  
* Improve model performance using deep learning  
* Support multilingual intent detection  
* Add persistent database (e.g., Firebase or SQLite)

**Setup Instructions**

1. Upload the entire \`autosort-ai\` folder to your Google Drive.  
2. Start with `classifier.ipynb` to train and save the model.  
3. Then open `main.ipynb` to run the inference pipeline interactively.
