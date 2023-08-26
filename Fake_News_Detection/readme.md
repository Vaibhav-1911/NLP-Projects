## Using NLP for Fake News Detection
In this project, I have built separate neural networks using RNN and LSTM and then compared the results for the two.

### Training Data
The training data consists of the following attributes. This is a tabular dataset.
- id: unique id for a news article
- title: the title of a news article
- author: author of the news article
- text: the text of the article; could be incomplete
- label: a label that marks the article as potentially unreliable

Link to the training dataset: https://www.kaggle.com/c/fake-news/data?select=train.csv

### Findings

LSTMs consist of an internal memory to store information for understanding long-term dependencies, which is crucial for a study like fake news detection as LSTMs may be able to capture patterns in fake news that RNNs might not. However, in my initial study, the RNN model performed better on tabular data than LSTM.

The next step is to identify if our data is less diverse or whether there is a lapse in the way we have trained our data in LSTM to understand why the LSTM model underperformed.
