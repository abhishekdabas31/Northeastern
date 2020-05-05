# Python

## A list is similar to an array in C++ 
>>> language = [a,[1,2,3,],b,cdefg, 1, True, False,'No']
You can put any kind of valuein a list - boolean, numeric , string, a list itself or a tuple

things you can do in a list :-
1. Accessing an entire list
>> list
2. Accessing a single item from the list
>> list1[3]
3. Slicing a python list
>> list1[1:4]
4. List is mutable
>> languages[2]='Java'
5. deleting a list
>>del languages[2]

## Tuples:
A tuple is an (immutable) ordered list of values. A tuple is in many ways similar to a list;
one of the most important differences is that tuples can be used as keys in dictionaries and as elements of sets, while lists cannot.

## List is mutable, Tuples are not 
>>> colors = ('red', 'green' , 'blue')
1. sincle element tuple
>> a=(1)
### We can perform these operations on a tuple just like we can on a list. The only differences that exist are because a tuple is immutable, so you can’t mess with a single item or a slice

## Python set, is just like the mathematical set
>> myset={3,1,2}
1. No duplicate values
2. It is unordered
there is no way we can use indexing to access or delete its elements
3. It is mutable (like List)

## Python dictionary holds key-value pairs.
>> mydict = {1:2,2:3,3:4}

# Numpy
Numpy is the core library for scientific computing in Python. It provides a high-performance multidimensional array object, and tools for working with these arrays.

## Arrays
A numpy array is a grid of values, all of the same type, and is indexed by a tuple of nonnegative integers. The number of dimensions is the rank of the array; the shape of an array is a tuple of integers giving the size of the array along each dimension.

`
e = np.random.random((2,2)) 
print(e)
[[0.57688929 0.54616642]
[0.28299089 0.10060504]]
`
## Series
A Series is a one-dimensional array of indexed data. One of the huge benefits of Pandas is that it supports both integer and label-based indexing, and provides a host of methods for performing operations involving the index. The first column is known as an index. And, each of the other columns corresponds to a Series. The first Series is called City, where the Olympics were held. The second Series is called the Edition, and this is the year the Olympics were held, and so on.


Source:-
https://pandas.pydata.org/pandas-docs/stable/getting_started/dsintro.html