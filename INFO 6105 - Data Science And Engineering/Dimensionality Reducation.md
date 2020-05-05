# What is Dimensionality Reduction?
Dimensionality reduction is simply, the process of reducing the dimension of your feature set. Your feature set could be a dataset with a hundred columns (i.e features) or it could be an array of points that make up a large sphere in the three-dimensional space. Dimensionality reduction is bringing the number of columns down to say, twenty or converting the sphere to a circle in the two-dimensional space.

## As the number of features increases, the model becomes more complex. The more the number of features, the more the chances of overfitting. A machine learning model that is trained on a large number of features, gets increasingly dependent on the data it was trained on and in turn overfitted, resulting in poor performance on real data, beating the purpose

# Avoiding overfitting is a major motivation for performing dimensionality reduction. The fewer features our training data has, the lesser assumptions our model makes and the simpler it will be. 
But that is not all and dimensionality reduction has a lot more advantages to offer, like
1. Less misleading data means model accuracy improves.
2. Less dimensions mean less computing. Less data means that algorithms train faster.
3. Less data means less storage space required.
4. Less dimensions allow usage of algorithms unfit for a large number of dimensions
5. Removes redundant features and noise.

# Feature Selection and Feature Engineering for dimensionality reduction
> Feature selection is the process of identifying and selecting relevant features for your sample. 
> Feature engineering is manually generating new features from existing features, by applying some transformation or performing some operation on them.

# Feature selection is the simplest of dimensionality reduction methods.

## We can make these simple manual feature selections and reduce the dimensionality when the relevance or irrelevance of certain features are obvious or common knowledge.
And when its not glaringly obvious, there are a lot of tools we could employ to aid our feature selection.
1. Heatmaps that show the correlation between features is a good idea.
2. So is just visualising the relationship between the features and the target variable by plotting each feature against the target variable.


# Now let us look at a few programmatic methods for feature selection from the popular machine learning library sci-kit learn, namely,
1. Variance Threshold  :  
Variance Threshold is a baseline approach to feature selection. As the name suggests, it drops all features where the variance along the column does not exceed a threshold value.
2. Univariate selection  :  
Univariate Feature Selection uses statistical tests to select features.
Univariate describes a type of data which consists of observations on only a single characteristic or attribute. Univariate feature selection examines each feature individually to determine the strength of the relationship of the feature with the response variable. Some examples of statistical tests that can be used to evaluate feature relevance are `Pearson Correlation, Maximal information coefficient, Distance correlation, ANOVA and Chi-square.` Chi-square is used to find the relationship between categorical variables and Anova is preferred when the variables are continuous.



#  Correlation is highly deceptive as it doesn’t capture strong non-linear relationships.

Source:- 
1.https://towardsdatascience.com/dimensionality-reduction-for-machine-learning-80a46c2ebb7e
