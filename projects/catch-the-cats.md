## Catch the CATs

_My first exploration of Feature Engineering_


### Project description

This is a [notebook](https://www.kaggle.com/code/yannansu/catch-the-cats-explore-feature-engineering) for the [Cat in the Dat](https://www.kaggle.com/c/cat-in-the-dat) competition on Kaggle.

> Is there a cat in your dat?
>
> A common task in machine learning pipelines is encoding categorical variables for a given algorithm in a format that allows as much useful signal as possible to be captured.
>
> Because this is such a common task and important skill to master, we've put together a dataset that contains only categorical features, and includes:
> - binary features
> - low- and high-cardinality nominal features
> - low- and high-cardinality ordinal features
> - (potentially) cyclical features

**The objective of this competition is to predict the value of the target column in the test set. In this project, I will particularly focus on feature encoding rather than tuning the model.**

### Aim & Methods
I started with a couple of questions:
1. What are the features in the dataset? What are their data types? Are there any missing values?
2. What are the distributions of the features?
3. How to encode binary features?
4. How to deal with the low- and high-cardinality nominal/ordinal features?
5. How to encode cyclical features?

Therefore, the analysis includes the following parts:
1. Exploratory Data Analysis
2. Feature Engineering
3. Model Training and Prediction

### Conclusions & Takeaways

- For binary features, we should always convert them to 0/1.
- For nominal features that have a clear order, we can use label encoding.
- For nominal features that have no clear order, we can use one-hot encoding. If they appear to be arrays of ASCII characters, we can convert them to numbers.
- For ordinal features with low-cardinality, we can set an order and use ordinal encoding.
- For ordinal features with high-cardinality that have no clear order, there are several ways to deal with it:
    - use label encoding
    - set an order by the frequency of appearance
    - if they happen to be ASCII characters, convert them to numbers, and then add them together, join them together, or create two columns for the first and second characters.

Things to try in the future:
- encode cyclical features with sine and cosine transformations for day and month columns
- compare the weights of the features in the model
- reduce the number of features

_For more details see [My Notebook on Kaggle](https://www.kaggle.com/code/yannansu/catch-the-cats-explore-feature-engineering)._
