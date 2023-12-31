---
# SMS/Email Spam Classifier
![image](https://github.com/adit2005/SMS-SPAM-CLASSIFIER/assets/119931302/a4ca8357-68f2-408d-96a6-f201ec44dbbc)


This project is a comprehensive SMS/Email Spam Classifier built using Python and various machine learning techniques. The goal of this project is to classify text messages as either spam or not spam (ham).

## Project Structure

The project consists of the following key files and components:

- **app.py**: The main Streamlit application file that allows users to input text messages and get predictions.

- **model.pkl**: A pickled file containing the trained Multinomial Naive Bayes (MNB) machine learning model for spam classification.

- **vectorizer.pkl**: A pickled file containing the TF-IDF vectorizer used for text feature extraction.

- **sms-spam-detection.ipynb**: A Jupyter Notebook containing the code for data preprocessing, model training, and evaluation.

- **README.md**: This comprehensive documentation file that covers both the Streamlit app and the Jupyter Notebook.

## Getting Started

To run the project, follow these steps:

1. Install the necessary Python libraries by running:

   ```bash
   pip install streamlit scikit-learn nltk pandas xgboost
   ```

2. Clone or download this repository to your local machine.

3. Navigate to the project directory.

4. Download NLTK's stopwords dataset by adding the following code snippet to the beginning of the `app.py` file:

   ```python
   import nltk
   nltk.download('stopwords')
   ```

5. Run the Streamlit app.

6. Access the app in your web browser by following the provided URL.

## Usage

### Streamlit App (`app.py`)

1. Open the Streamlit app in your web browser.

2. Enter a text message that you want to classify in the provided text area.

3. Click the "Predict" button.

4. The app will display whether the input message is classified as "Spam" or "Not Spam" based on the trained Multinomial Naive Bayes (MNB) model's prediction.

### Jupyter Notebook (`sms-spam-detection.ipynb`)

1. Open the Jupyter Notebook to explore the code for data preprocessing, model training, and evaluation.

2. Follow the step-by-step instructions in the notebook to understand how the machine learning model was developed.

## Model Information

The Streamlit app uses a trained Multinomial Naive Bayes (MNB) model for spam classification. The model has been evaluated for accuracy and precision.

## Model Improvement

The project may include methods for improving the model's performance, such as changing the `max_features` parameter of TF-IDF. You can experiment with these techniques to optimize the model further.

## Ensemble Methods

The project also demonstrates the use of ensemble methods, such as a Voting Classifier and a Stacking Classifier, to combine the strengths of multiple machine learning models for improved classification accuracy.

## Saving the Model

The trained TF-IDF vectorizer and Multinomial Naive Bayes (MNB) model can be saved for future use using the `pickle` library. You can find the saved models as `vectorizer.pkl` and `model.pkl`.

---
