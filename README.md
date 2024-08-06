
# Email/SMS Spam Classifier

This repository contains a Streamlit web application that classifies Email/SMS messages as spam or not spam using a machine learning model. The application preprocesses the input text, vectorizes it, and then uses a trained model to predict whether the message is spam.

## Overview

## Features

- **Text Preprocessing**: Converts text to lowercase, removes special characters, stopwords, and applies stemming.
- **Vectorization**: Uses TF-IDF vectorizer to convert text into numerical format.
- **Spam Classification**: Predicts whether the message is spam or not using a pre-trained machine learning model.

## Prerequisites

- Python 3.7 or higher
- Streamlit
- NLTK
- Scikit-learn
- Pickle files (`vectorizer.pkl` and `model.pkl`) containing the trained TF-IDF vectorizer and machine learning model, respectively.

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/spam-classifier.git
    cd spam-classifier
    ```

2. **Create and activate a virtual environment**:
    ```sh
    python -m venv venv
    venv\Scripts\activate
    ```

3. **Install the required packages**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Download NLTK data**:
    ```sh
    python -m nltk.downloader stopwords punkt
    ```

5. **Ensure you have the `vectorizer.pkl` and `model.pkl` files**:
    - Place `vectorizer.pkl` and `model.pkl` in the root directory of the project.

## Usage

1. **Run the Streamlit app**:
    ```sh
    streamlit run app.py
    ```

2. **Open your web browser**:
    - Go to `http://localhost:8501`.

3. **Classify Messages**:
    - Enter the message in the provided text area.
    - Click on the "Predict" button to see if the message is spam or not.

## File Structure

- `app.py`: The main Streamlit application file.
- `vectorizer.pkl`: Pickle file containing the trained TF-IDF vectorizer.
- `model.pkl`: Pickle file containing the trained machine learning model.
- `requirements.txt`: List of required Python packages.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any features, bug fixes, or enhancements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
    

