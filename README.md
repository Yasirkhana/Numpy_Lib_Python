# NUMPY LIBRARY
```python
# NUmpy = Numerical python 
## It is use for scientific calculations

import numpy as np 
a1 = np.array([1,5,3,5])
print(type(a1))
print(a1)
```

    <class 'numpy.ndarray'>
    [1 5 3 5]
    


```python
a2 = np.array([[5,3,42,53,5],[34,45,2,5,15]])
```


```python
a2
```




    array([[ 5,  3, 42, 53,  5],
           [34, 45,  2,  5, 15]])




```python
a3 = np.zeros((4,4))
```


```python
a3
```




    array([[0., 0., 0., 0.],
           [0., 0., 0., 0.],
           [0., 0., 0., 0.],
           [0., 0., 0., 0.]])




```python
a4 = np.full((3,5),(555))
```


```python
a4
```




    array([[555, 555, 555, 555, 555],
           [555, 555, 555, 555, 555],
           [555, 555, 555, 555, 555]])




```python
a5 = np.arange(10,100,2)   # to print specific range in array
```


```python
a5
```




    array([10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42,
           44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76,
           78, 80, 82, 84, 86, 88, 90, 92, 94, 96, 98])




```python
a6 = np.random.randint(1,100,50)    # make array with random number from range(1 to 100) ( total number = 50)
```


```python
a6
```




    array([90, 36, 26, 77, 60,  9, 19, 94, 95, 17, 36, 67, 70, 15,  8, 72, 21,
           33, 55, 47,  2, 69, 50, 24, 43, 58,  7, 51, 71, 38, 67, 62, 62, 15,
           42,  4,  9,  9, 19, 31, 25, 74, 84, 15, 18, 69, 53, 15, 16, 65])




```python

a2.shape   # shows the shape of array (e.g : 2 row, 5 cols)
```




    (2, 5)




```python
a6.shape 

```




    (50,)




```python
a6.shape = (1,50)    # reshaped a6 from (50,1) to (1,50)
```


```python
a6.shape
```




    (1, 50)




```python
a6
```




    array([[90, 36, 26, 77, 60,  9, 19, 94, 95, 17, 36, 67, 70, 15,  8, 72,
            21, 33, 55, 47,  2, 69, 50, 24, 43, 58,  7, 51, 71, 38, 67, 62,
            62, 15, 42,  4,  9,  9, 19, 31, 25, 74, 84, 15, 18, 69, 53, 15,
            16, 65]])




```python
n1 = np.array([1,4,5,2])
n2 = np.array([5,74,35,12])

```


```python
np.vstack((n1,n2))           #  join Two or more arrays of same dimentions
                            # 3 types of stack
                            # Vstack = vertical stack
                            # hstack = horizontal stack
                            # cstack = column stack
```




    array([[ 1,  4,  5,  2],
           [ 5, 74, 35, 12]])




```python
np.intersect1d(n1,n2)   # for intersection 
```




    array([5])




```python
np.union1d(n1,n2)       # union of two array
```




    array([ 1,  2,  4,  5, 12, 35, 74])




```python
np.setdiff1d(n1,n2)     # difference btw two array
```




    array([1, 2, 4])




```python
np.add(n1,n2)            # add to array of same dimention
```




    array([ 6, 78, 40, 14])




```python
np.sum([n1,n2])          # sum all elements of two array
```




    138




```python
np.sum([n1,n2],axis = 1)       # Horizontal sum
```




    array([ 12, 126])




```python
np.sum([n1,n2],axis = 0)      # Vertical sum
```




    array([ 6, 78, 40, 14])




```python
s1 = np.array([1,5,6,8,9,2])       # saving array
np.save("MyArr",s1)
```


```python

np.load("Myarr.npy")                  # loading array
```




    array([1, 5, 6, 8, 9, 2])




```python

```
