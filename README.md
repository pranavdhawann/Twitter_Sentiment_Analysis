# Twitter Sentiment Analysis

This project performs sentiment analysis on Twitter data using various machine learning models, including Naive Bayes, Random Forest, and an LSTM-based neural network. The goal is to classify tweets into three sentiment categories: Positive, Neutral, and Negative.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Evaluation](#evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/pranavdhawann/Twitter_SA.git
    cd Twitter_SA
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. If using Google Colab, mount your Google Drive:
    ```python
    from google.colab import drive
    drive.mount('/content/gdrive')
    ```

## Usage

1. Unzip the data file:
    ```bash
    unzip /content/gdrive/MyDrive/SA.zip -d .
    ```

2. Load the data and run the analysis:
    ```python
    import pandas as pd

    path = '/content/Twitter_Data.csv'
    data = pd.read_csv(path)
    ```

3. Follow the steps in the notebook or script to preprocess the data, train the models, and evaluate their performance.

## Data

The dataset `Twitter_Data.csv` contains the following columns:
- `clean_text`: The preprocessed text of the tweets.
- `category`: The sentiment label (-1 for Negative, 0 for Neutral, 1 for Positive).

## Models

Three models are used in this project:
1. **Naive Bayes**: A simple yet effective classifier for text data.
2. **Random Forest**: An ensemble method that improves performance by combining multiple decision trees.
3. **LSTM-based Neural Network**: A deep learning model suitable for sequential data like text.

## Evaluation

The models are evaluated using:
- **Accuracy**: The percentage of correctly classified instances.
- **Classification Report**: Precision, recall, and F1-score for each class.

## Results

### Naive Bayes
- Accuracy: 74.01%
- Precision, Recall, F1-score: See classification report in the notebook.

### Random Forest
- Accuracy: 84.54%
- Precision, Recall, F1-score: See classification report in the notebook.

### LSTM-based Neural Network
- Accuracy: 94.71%
- Precision, Recall, F1-score: See classification report in the notebook.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
