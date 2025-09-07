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
<img width="464" height="257" alt="image" src="https://github.com/user-attachments/assets/3976d621-220f-4902-a326-5a4fe0ad768d" />

### How i made it:
For the normalizaiton problem, i first inputted the numpy library using the "import numpy as np" code so that the following codes can use a high performance array called ndarray and so that i can also use the mathematical functions like "mean()" and "std()" which can help the code so that i can easily process the mean and standard deviations of the array. Next i generated a 5 x 5 array that have random values using the code "np.random.random(5,5)". Next i calculated the normalized score using the formula "(X - X.mean())/ X.std()" and set the values into the array "X_normalized". Lastly i saved the "X_normalied" into an .npy file to store the array and displayed both of the original and the normalized array so that i can check if the the output is correct.

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
<img width="437" height="252" alt="image" src="https://github.com/user-attachments/assets/788c1aed-49fc-4ada-a272-cd67f075a453" />

### How i made it:
For the divisible by 3 problem, i first inputted the numpy library using the "import numpy as np" code so that the following codes can use a high performance array called ndarray. Then i listed all of the numbers ranging from 1 to 100 using the code "list(range)1-101))" and stored it into variable "num" as a list. Next, i turned the list into a ndarray using the code "np.array(num)" and stored it to variable "A". Then i used the code "A ** 2" to raise their exponents by 2 to square all of the numbers. Then i reshaped the array using the code "reshape(10,10) to reshape the array into a 10 x 10 ndarray. Then used the code "A[A % 3 == 0]" in which the code divides each element by 3 and checks if the remainder is 0. If its true then i inputs the number into the array. i stored the array into "div_by_3" for further uses since i saved as an .npy file to easily store the data locally. Lastly i displayed the array so that i can further inspect if the output is correct.

### Output
<img width="818" height="100" alt="image" src="https://github.com/user-attachments/assets/4d47a1ed-9154-4797-b77a-2a4b9ba1c7fc" />

### Lesson learned
Through solving this problem, i advanced my skills in manipulating each element of the array in a large scale, from generating specific integers, turning a list into an ndarray, squaring each element of the array and leaving only the elements divisible by 3 in the array.
