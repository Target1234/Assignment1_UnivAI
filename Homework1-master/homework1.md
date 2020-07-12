# Homework 1

Foundations Program, ktf-c1

**Due** Sun July 12th 5PM IST

## Problem 1

(**this is a long question and involves a lot of reading, so start ASAP**)

In the data folder below, you will find multiple Shakespeare plays. You will compute the cosine similarity of these plays to find which of these plays are similar and which are different.

The definition is provides in the first 3 paras of this [Cosine Similarity](https://en.wikipedia.org/wiki/Cosine_similarity) article on wikipedia.

Read the slides and notes (notebooks) in both the `DundersOperators` and `SoftwareDevelopment` repositories.

You will define a vector class using the tests (and any additional tests you might like to add) from the `vector4.py` in repository SoftwareDevelopment. However, you must replace the list based implementation by an implementation using numpy arrays, and make sure the tests still run. Note that this will result in the removal of a lot of code, rather than the addition of code, as numpy makes things simple for you.

`np.dot` will be your ticket to obtaining dot products. But remember that you must divide the dot product by the magnitudes of both the vectors to obtain the cosine similarity. Thus you must define a method to compute the magnitude ( also called norm or length) of the vector in your class and test it. Add tests!

You will compute vectors from each play by parsing the text of the play into words, and then storing the counts of these words in a vector. 

Remove the most common english words like 'and', 'it' and simililar from each play (this should be the same set of words for all plays). You can do this by sorting the order of the words obtained by their frequency. Unify all the words from all the plays into a set (using the union of the individual play sets), and then convert the resultant set into a list to create the vocabulary. For each word in the vocabulary, see how often that word occured in a play..this is the component of that word for that play. It might look something like this:

```
war    peace    death    laughter .....
15     3        10       2        (Julius Casear)
1      5        1        10       (Midsummer's Night Dream)
```

Now compute the cosine similarity for each pair of plays in the data folder. The reason you computed one vocabulary by unioning the plays individual vocabularies is to be able to have a (a) systematic and (b) identical-dimensioned way of computing the dot product for this similarity

How would you (just describe it in words) give a reasonable answer if someone asked you which play was the saddest play?

## Problem 2

In this problem we will learn some new numpy functions which will be used in the future!
These functions are highly used in many machine learning algorithms

### numpy.ones()

try creating an array of given shape, 2 and type int , with ones.



```python
# your code here
```


try creating an array of given shape, [3,3] and type int , with ones.



```python
# your code here
```


### numpy.zeros()

try creating an array of given shape, 4 and type int , with zeros.



```python
# your code here
```


try creating an array of given shape, [2,2] and type int , with zeros.



```python
# your code here
```


Similarly, try updating the data type to float



```python
# your code here
```


### np.dtype()

Create a datatype object of int16



```python
# your code here
```


### numpy.concatenate()



```python
import numpy as np
a = np.array([[1,2],[3,4]]) 
b = np.array([[5,6],[7,8]]) 
```


concatenate the given two arrays into a single array along the axis 0



```python
# your code here
```


concatenate the given two arrays into a single array along the axis 1



```python
# your code here
```


### numpy.flatten()



```python
## Flatten the given 2d numpy array into 1d array
a = np.array([[1, 2, 3], [2, 4, 5], [1, 2, 3]]) 
```




```python
# your code here
```


### numpy.ravel()

similarly flatten the given previous array to 1d array using numpy.ravel()



```python
# your code here
```

