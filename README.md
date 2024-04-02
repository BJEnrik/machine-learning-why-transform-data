<h1 style="color:#5A59A8">Executive Summary</h1>

<div style="text-align: justify">Getting accurate results is the goal of every machine learning project. But feeding data as it is to a model does not always give the desired outcome. And doing so will introduce certain biases to your machine learning model as it learns. One way to mitigate this problem is by feature transformation or feature scaling. But how would you exactly know what feature transformation technique to use in certain situations?</div>
&nbsp

<div style="text-align: justify">Data is transformed to make it better-organized. Transformed data may be easier for both humans and computers to use. [11] Feature transformation is an essential data preprocessing technique that ensures all of our metrics are uniform which allows for better model performance. This also ensures that algorithms moves smoothly and is applied and updated at the same rate for all features.</div>
&nbsp

<div style="text-align: justify">For this notebook, we will explore nine (9) data transformation techniques and how these techniques boosts model performance. These techniques will be divided into three main categories namely: Function Transformation, Power Transformation, and Other Transformation. </div>
&nbsp


<h1 style="color:#5A59A8">Introduction</h1>

<h2 style="color:#E14C92">Transformation of Features</h2>

<h3 style="color:#0094AD">What is Feature Transformation?</h3>

1. <div style="text-align: justify">It is a technique by which we can boost our model performance. Feature transformation is a mathematical transformation in which we apply a mathematical formula to a particular column(feature) and transform the values which are useful for our further analysis. [1]</div>


2. <div style="text-align: justify">It is also known as Feature Engineering, which is creating new features from existing features that may help in improving the model performance. [1]</div>


3. <div style="text-align: justify">It refers to the family of algorithms that create new features using the existing features. These new features may not have the same interpretation as the original features, but they may have more explanatory power in a different space rather than in the original space. [1]</div>


4. <div style="text-align: justify">This can also be used for Feature Reduction. It can be done in many ways, by linear combinations of original features or by using non-linear functions. [1]</div>


5. <div style="text-align: justify">It helps machine learning algorithms to converge faster. [1]</div>

<h3 style="color:#0094AD">What are the Different Types Transformation?</h3>

1. <div style="text-align: justify"> Function Transformation </div>
2. <div style="text-align: justify"> Power Transformation </div>
3. <div style="text-align: justify"> Other Transformation </div>

<h2 style="color:#E14C92">Function Transformation</h2>

**Log Transformation**

<div style="text-align: justify">The log transformation is, arguably, the most popular among the different types of transformations used to transform skewed data to approximately conform to normality. [2]</div>

**Reciprocal Transformation**

<div style="text-align: justify">The reciprocal transformation is defined as the transformation of x to 1/x. The transformation has a dramatic effect on the shape of the distribution, reversing the order of values with the same sign. The transformation can only be used for non-zero values. [3]</div>

**Square Transformation**

<div style="text-align: justify">The square root, x to x^(1/2) = sqrt(x), is a transformation with a moderate effect on distribution shape: it is weaker than the logarithm and the cube root. It is also used for reducing right skewness, and also has the advantage that it can be applied to zero values. Note that the square root of an area has the units of a length. It is commonly applied to counted data, especially if the values are mostly rather small. [4]</div>

**Square Root Transformation**

<div style="text-align: justify">The square, x to x^2, has a moderate effect on distribution shape and it could be used to reduce left skewness. In practice, the main reason for using it is to fit a response by a quadratic function y = a + b x + c x^2. [4]</div>

<h2 style="color:#E14C92">Power Transformation</h2>

**Box-Cox Transformation**

<div style="text-align: justify">A Box Cox transformation is a transformation of non-normal dependent variables into a normal shape. Normality is an important assumption for many statistical techniques; if your data isn’t normal, applying a Box-Cox means that you are able to run a broader number of tests. [6]</div>

**Yeo-Johnson Transformation**

<div style="text-align: justify">The Yeo-Johnson family of transformations modifies and generalizes the Box-Cox family to handle data where the smallest value of y may be zero or negative. For non-negative values of y, it finds the Box-Cox transformation of y+1. [7]</div>

<h2 style="color:#E14C92">Other Transformation</h2>

**Normalization and Standardization**
1. <div style="text-align: justify">Normalization is used when the data doesn't have Gaussian distribution whereas Standardization is used on data having Gaussian distribution. [8]</div>

2. <div style="text-align: justify">Normalization scales in a range of [0,1] or [-1,1]. Standardization is not bounded by range. [8]</div>

3. <div style="text-align: justify">Normalization is highly affected by outliers. Standardization is slightly affected by outliers. [8]</div>

4. <div style="text-align: justify">Normalization is considered when the algorithms do not make assumptions about the data distribution. Standardization is used when algorithms make assumptions about the data distribution. [8]</div>

**Min-Max Scaling**
1. <div style="text-align: justify">MinMax Scaler is one of the most popular scaling algorithms. It transforms features by scaling each feature to a given range, which is generally [0,1], or [-1,-1] in case of negative values. [9]</div>

2. <div style="text-align: justify">It subtracts the mean of the column from each value and then divides by the range, i.e, max(x)-min(x). [9]</div>

3. <div style="text-align: justify">This scaling algorithm works very well in cases where the standard deviation is very small, or in cases which don’t have Gaussian distribution. [9]</div>

**Quantile and Median Scaling**
1. <div style="text-align: justify">When scaling variables to the median and quantiles, the median value is removed from the observations and the result is divided by the inter-quartile range (IQR). The IQR is the range between the 1st quartile and the 3rd quartile, or, in other words, the range between the 25th quantile and the 75th quantile. [10]</div>

2. <div style="text-align: justify">This method is known as robust scaling because it produces more robust estimates for the center and value range of the variable, and is recommended if the data contains outliers. [10]</div>

<h2 style="color:#E14C92">Summary of Transformations</h2>

1. Normalization and Standardization
2. Min-Max Scaling
3. Robust Scaling
4. Log Transformation
5. Reciprocal Transformation
6. Square Transformation
7. Square Root Transformation
8. Quantile Transformation
9. Box-Cox Transformation
10. Yeo-Johnson Transformation


