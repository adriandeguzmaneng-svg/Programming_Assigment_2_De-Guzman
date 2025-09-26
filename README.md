# Programming_Assigment_2_De-Guzman
This Programming Assignment contains the python code solution to the Normalization and Divisible by 3 problems made by Adrian S. De Guzman from 2 ECE - A as a assigment for his course ECE 2112 - Advanced Computer Programming and Algorithms
___
## Normaliation Problem

### Overview
Normalization is one of the most basic preprocessing techniques in
data analytics. This involves centering and scaling process. Centering means subtracting the data from the
mean and scaling means dividing with its standard deviation. Mathematically, normalization can be
expressed as:

<img width="164" height="72" alt="image" src="https://github.com/user-attachments/assets/9b534cfe-f78a-48c4-876b-2295ba181020" />

In this problem, we are tasked to create a random 5 x 5 ndarray and store it to variable X. Normalize X and Save our normalized ndarray as X_normalized.npy

### Code
```python
import numpy as np
X = np.random.random((5,5))
X_normalized = (X - X.mean())/ X.std()
X_normalized
np.save("X_normalized.npy",X_normalized)
print("Original Array:",X)
print()
print("Normalized Array:",X_normalized)
```
### How does it work
These lines initializes the array by importing the library and generating the array
```python
import numpy as np #imports the numpy array for array manipulation
X = np.random.random((5,5)) #generates a 5x5 array with random values inside
```
This line performs the normalizaiton formula to the whole array
```python
X_normalized = (X - X.mean())/ X.std() #normalized value of each value in the array
```
These lines saves and displays the array for the user
```python
np.save("X_normalized.npy",X_normalized) #saves the array into a .npy file format
print("Original Array:",X) #prins the original array for comparison
print() #prints a line for easier visualizaiton
print("Normalized Array:",X_normalized) #displays the normalized array
```
### Output
<img width="891" height="311" alt="image" src="https://github.com/user-attachments/assets/4979e375-5773-47fd-b2ea-1a24b10a06d7" />

(The output is not always the same since the code generates a random and brand new variables each time)

### Lesson Learned
Through solving the Normalization Problem, i advanced my skills in using pre-defined functions as well as using quite complex mathematical equations using only codes. Through this project,i also learned to expand my knowledge in ndarrays in which i manipulated an ndarray mutiple times such as filling it with random values, performing a large equation on each element of the array and save an array into an .npy file to easily store the data locally.
*** 
## Divisble by 3 Problem

### Overview
For this project, we are tasked to create a 10 x 10 ndarray which contains the square of the first 100 integers.
<img width="457" height="164" alt="image" src="https://github.com/user-attachments/assets/eb8a963d-f72d-445f-aa45-73a798c41668" />

From that ndarray, we needed to determine all the elements that are divisible by 3 and save the result as div_by_3.npy.

### Code
```python
import numpy as np
num = list(range(1, 101))
A = np.array(num)
A = A ** 2
A.reshape(10,10)
div_by_3 = A[A % 3 == 0]
np.save("div_by_3.npy",div_by_3)
div_by_3
```
### How does it work?
These lines initializes the library and the array
```python
import numpy as np #imports the numpy array for array manipulation 
num = list(range(1, 101)) #creates a list in which the number are from 1-100
A = np.array(num) #turns the list into an 1 dimensional ndarray
A = A ** 2 #squares each value of the array or raises the exponent into 2
A.reshape(10,10) #reshapes the 1D array into array into 10 x 10 2D array
```
This lines perfoms the formula for the required values of the array
```python
div_by_3 = A[A % 3 == 0] #divives the value by 3 and checks if he remainder of the quotient is 0 and puts it in the array
```
This lines saves and displays the array for the user
```python
np.save("div_by_3.npy",div_by_3) #saves the array into a .npy file format
div_by_3 #displays the array
```
### Output
<img width="818" height="100" alt="image" src="https://github.com/user-attachments/assets/4d47a1ed-9154-4797-b77a-2a4b9ba1c7fc" />

### Lesson learned
Through solving this problem, i advanced my skills in manipulating each element of the array in a large scale, from generating specific integers, turning a list into an ndarray, squaring each element of the array and leaving only the elements divisible by 3 in the array.
___
## Version 2
