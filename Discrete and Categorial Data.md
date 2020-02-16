 ## Machine Learning algorithms cannot work directly with categorical data and you do need to do some amount of engineering and transformations on this data before you can start modeling on your data.

# Categorical Data
A categorical data is usually in the form of discrete values which belongs to a specific finite set of categories. 
These are also known as classes or labels in the contect of attributes or variables which are to be predicted by a model. 
These values can be text or numeric in nature. There are two major classes of categorical data:
Normal :-
There is no concept of ordering amongst the values of that attribute.
Example- Weather___ we have six major classes or categories in this particular scenario without any concept or notion of order (windy doesn’t always occur before sunny nor is it smaller or bigger than sunny).
ordinal :- 
This one has some sense or notion of order amongst its values. 
Exmaple:- Shirt size____ It is quite evident that order or in this case ‘size’ matters when thinking about shirts (S is smaller than M which is smaller than L and so on).

# Engineering on Categorical Data
A lot of advancements have been made in various machine learning frameworks to accept complex categorical data types like text labels. Typically any standard workflow in feature engineering involves some form of transformation of these categorical values into numeric labels and then applying some encoding scheme on these values. We load up the necessary essentials before getting started.

# Encoding Categorical Attributes
If you remember what we mentioned earlier, typically feature engineering on categorical data involves a transformation process which we depicted in the previous section and a compulsory encoding process where we apply specific encoding schemes to create dummy variables or features for each category\value in a specific categorical attribute.
You might be wondering, we just converted categories to numerical labels in the previous section, why on earth do we need this now? The reason is quite simple. Considering video game genres, if we directly fed the GenreLabel attribute as a feature in a machine learning model, it would consider it to be a continuous numeric feature thinking value 10 (Sports) is greater than 6 (Racing) but that is meaningless because the Sports genre is certainly not bigger or smaller than Racing, these are essentially different values or categories which cannot be compared directly. Hence we need an additional layer of encoding schemes where dummy features are created for each unique value or category out of all the distinct categories per attribute.

# One-hot Encoding Scheme
Considering we have the numeric representation of any categorical attribute with m labels (after transformation), the one-hot encoding scheme, encodes or transforms the attribute into m binary features which can only contain a value of 1 or 0. Each observation in the categorical feature is thus converted into a vector of size m with only one of the values as 1 (indicating it as active). 

# Dummy Coding Scheme
The dummy coding scheme is similar to the one-hot encoding scheme, except in the case of dummy coding scheme, when applied on a categorical feature with m distinct labels, we get m - 1 binary features. Thus each value of the categorical variable gets converted into a vector of size m - 1. The extra feature is completely disregarded and thus if the category values range from {0, 1, …, m-1} the 0th or the m - 1th feature column is dropped and corresponding category values are usually represented by a vector of all zeros (0). Let’s try applying dummy coding scheme on Pokémon Generation by dropping the first level binary encoded feature (Gen 1).


Source- 
https://towardsdatascience.com/understanding-feature-engineering-part-2-categorical-data-f54324193e63