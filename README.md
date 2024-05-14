# Fake News Detection with Python

This project aims to build a machine learning model to accurately classify news articles as real or fake using Python. We leverage a political dataset containing news articles and labels indicating whether each article is real or fake.

## Dataset

The dataset used for this project can be found [here](https://github.com/GeorgeMcIntire/fake_real_news_dataset). It consists of a CSV file named `news.csv` with the following structure:

- Column 1: News ID
- Column 2: Title
- Column 3: Text
- Column 4: Label (REAL or FAKE)

The dataset contains 7796 news articles.

## Methodology

1. **Data Preprocessing**: We preprocess the text data by tokenizing, removing stop words, and vectorizing using TF-IDF (Term Frequency-Inverse Document Frequency).

2. **Model Selection**: We utilize a Passive Aggressive Classifier for training the model. This algorithm is suitable for online learning, remaining passive for correct classifications and turning aggressive for incorrect ones.

3. **Model Training**: We fit the Passive Aggressive Classifier to the preprocessed data to learn the patterns between news content and their labels.

4. **Model Evaluation**: We evaluate the trained model's performance using accuracy metrics to measure its ability to correctly classify news articles.

## Results

After training and evaluating the model, we achieved an accuracy of 92.82%, demonstrating the effectiveness of the approach in detecting fake news.So with this model, we have 589 true positives, 587 true negatives, 42 false positives, and 49 false negatives.

![Output](file:///Users/pratyekthumula/Downloads/WhatsApp%20Image%202024-05-14%20at%2013.52.41.jpeg)


## Usage

To replicate the project:

1. Clone the repository containing the dataset.
2. Install the necessary Python libraries (e.g., pandas, scikit-learn).
3. Use the provided Jupyter Notebook or Python script to preprocess the data, train the model, and evaluate its performance.

## Conclusion

Fake news detection is a critical task in today's digital age. By leveraging machine learning techniques like the Passive Aggressive Classifier, we can build models capable of discerning between real and fake news articles, contributing to the fight against misinformation.
