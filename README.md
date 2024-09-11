This programming assignment focuses on applying normalization techniques in data analytics using Python. It involves creating and manipulating ndarray and experimenting with their functions. The goal is to provide hands-on experience with both the theory and practical implementation of normalization methods in Python.


Reference:
```
[1]   import numpy as np
[2]   X = np.random.rand(5, 5)                            
[3]        
[4]   mean = X.mean()                                      
[5]   standard_deviation = X.std()
[6]
[7]   X_normalized = (X - mean) / standard_deviation      
[8]
[9]   np.save('X_normalized.npy', X_normalized)          
[10]
[11]  X_normalized
```

<p align="center"> 
NORMALIZATION PROBLEM
</p>  

In order to utilize the Numerical Python library we first need to first write the following (line [1]): 
```
import numpy as np
```
In the second line of the text involves the creation of a 5x5 ndarray with randomly generated integers inside the array and this ndarray will be stored to the variable X.
```
X = np.random.rand(5,5)
```
The next two following lines ([4],[5]) involves the creation of functions that utilizes the library of numerical python. The functions utilized are ```.mean()``` and ```.std()``` and these functions are used to get the mean and standard deviation of the ndarray X.

And finally to the main course of this problem, the normalization. The equation for normalization is given as the following:

<p align="center">
  $Z = \frac{X - x̄}{\sigma}$
</p>  

Lastly, the next line of code involved saving the obtained normalized values in the ndarray as ```X_normalized.npy``` and printing it out. 
The output is shown as the following: 
```
array([[-0.15046758, -0.54418315,  1.02313319, -0.00463552, -1.1525935 ],
       [ 0.5957998 ,  1.6354055 ,  1.14896291,  0.40787044,  0.10829311],
       [ 0.26577843,  0.03382761, -1.31330459,  1.62113452, -0.35829203],
       [-1.79165435, -1.22178644, -0.32245622, -1.56558256,  0.17761454],
       [-1.76855556,  0.36928004,  1.04650279,  0.7619018 ,  0.99800682]])
```
---
---
 <p align="center"> DIVISIBLE BY 3 </p>

 Reference: 
 ```
[1]import numpy as np
[2]
[3]array = (np.arange(1, 101).reshape(10, 10) ** 2)   
[4]
[5]div_by_3 = array[array % 3 == 0]                  
[6]
[7]np.save('div_by_3.npy', div_by_3)        
[8]div_by_3                                     

```
Simillar to the first problem, we first write ```import numpy as np``` in order to utilize numerical python library

In the following line, we create an array that will store values that range from 1 to 100 using ```np.arange(1,101)```

it is then followed by the ```.reshape()``` method and inside the parenthesis we indicate the shape of the array.
we then use "**" otherwise known as the exponential syntax in order to get the square of the numbers inside the array.

A modulo function is then created in line [5] with a variable name of "div_by_3" that will find integers divisible by 3

At line [7] "div_by_3" is saved as "div_by_3.npy" at the disk

Line [8] is where the output gets displayed.



   
