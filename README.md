# Bank-Note-Authentication-using-TensorFlow-2.0

In this notebook, we utilise the effectiveness of Neural Nets for some Bank notes data.

We use the [Bank Authentication Data Set](https://archive.ics.uci.edu/ml/datasets/banknote+authentication) from the UCI repository.

The data consists of 5 columns:

- variance of Wavelet Transformed image (continuous)
- skewness of Wavelet Transformed image (continuous)
- curtosis of Wavelet Transformed image (continuous)
- entropy of image (continuous)
- class (integer)

Where class indicates whether or not a Bank Note was authentic.

The data is explored using **seaborn** by creating countplot and pairplot for the data with respect to **class**.

The features are scaled and converted to numeric. A **DNN classifier** estimator is instantiated and then trained with an input function defined for training in accordance with suitable *batch size*,*steps*,*hidden units*,etc.

Then the trained model is evaluated for performance with predictions on the test data using the input function defined for prediction.

As a result, the DNN classifier performs exceptionally well with an accuracy of *approx. 98%* and extremely accurate precision and recall.
