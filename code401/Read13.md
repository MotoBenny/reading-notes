# Linear regression in python scikit-learn

### Scikit-learn 
A python module for machine learning.

 >The first step is to import the required Python libraries into Ipython Notebook.

![Explore 1](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Explore-1.png)

*thoughts, up to now, this method of processing data looks quite similar to pandas.*
example being ``` boston.feature_names ``` producing the names on dataset.

Grabing the linearRegression module

> First, I am going to import linear regression from sci-kit learn module. Then I am going to _[drop](http://pandas.pydata.org/pandas-docs/dev/generated/pandas.DataFrame.drop.html)_ the price column as I want only the parameters as my X values. I am going to store linear regression object in a variable called _lm_.

![Skitlearn linear model](https://bigdata-madesimple.com/wp-content/uploads/2016/04/Skitlearn-linear-model1.png)

### Training and Validation
*This is awesome stuff! I didnt realize we would touch on ML here in 401.*

>In practice you wont implement linear regression on the entire data set, you will have to split the data sets into [training and test](http://www.researchgate.net/post/Whats_the_difference_between_training_set_and_test_set) data sets. So that you train your model on training data and see how well it performed on test data.

>_How not to do train-test split_:

![train-test split](https://bigdata-madesimple.com/wp-content/uploads/2016/04/train-test-split.png)

*Interesting here, but the point being made that you can accidentally train on one thing and test on another is a prime example of why not to do this.*

>You can create training and test data sets manually, but this is not the right way to do, because you may be training your model on less expensive houses and testing on expensive houses.

I think this entire subject here is certainly much too deep for this single blog post, ll have to find some more learning tools and understanding here. 