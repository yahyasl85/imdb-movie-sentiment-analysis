# imdb-movie-sentiment-analysis
The goal of this project is to build a sentiment analysis model that can classify movie reviews as positive or negative.  General Methodology:  The project uses a recurrent neural network (RNN) with Long Short-Term Memory (LSTM) layers to achieve this goal
# Movie Review Sentiment Analysis

This project aims to build a sentiment analysis model that can classify movie reviews as positive or negative.

## Methodology

The project uses a recurrent neural network (RNN) with Long Short-Term Memory (LSTM) layers to achieve this goal. It involves the following steps:

1. **Data Preparation:**
    - The project uses the IMDB movie review dataset, which is a collection of movie reviews labeled as positive or negative.
    - The reviews are preprocessed by converting them into numerical representations using techniques like Bag-of-Words and One-Hot Encoding.
    - The data is then padded to ensure all reviews have the same length.

2. **Model Building:**
    - An RNN model with LSTM layers is created using the Keras library.
    - The model consists of an embedding layer, an LSTM layer, and a dense layer with a sigmoid activation function for binary classification.

3. **Model Training:**
    - The model is trained on the preprocessed IMDB dataset using the `binary_crossentropy` loss function and the `rmsprop` optimizer.
    - The training process involves feeding the model with batches of movie reviews and their corresponding labels.

4. **Model Evaluation:**
    - The model's performance is evaluated on a validation set to assess its accuracy and generalization ability.
    - Metrics like accuracy and loss are used to measure the model's performance.

5. **Prediction:**
    - Once trained, the model can be used to predict the sentiment of new movie reviews.
    - The input review is preprocessed and fed into the model, which outputs a probability score indicating whether the review is positive or negative.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Keras
- NumPy

## Usage

1. Clone the repository: `git clone <repository_url>`
2. Install the required libraries: `pip install -r requirements.txt`
3. Run the Jupyter notebook: `jupyter notebook sentiment_analysis.ipynb`

## Results

The model achieves an accuracy of around 85% on the validation set.

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
