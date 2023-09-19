# ***matrix-multiplication***

### _2D_ matrix multiplication using `python3`

![Basic_MMM](https://github.com/pyamin1878/matrix-multiplication/assets/11963396/efac9a8d-70e0-4646-8bbf-c7edf4c9823b)



## explicit with nested loops
```python
#input two matrices and label them

matrix_1 = [[1,2,3],
            [4,5,6],
            [7,8,9]]
matrix_2 = [[0,1,2],
            [3,4,5],
            [6,7,8]]

res = [[0 for x in range (3)] for y in range(3)]

# nested for loops

for i in range(len(matrix_1)):
    for j in range(len(matrix_2[0])):
        for k in range(len(matrix_2)):

# resulted matrix
            
            res[i][j] += matrix_1[i][k] * matrix_2[k][j]

print(res)
```
## `numpy`
```python
# input two matrices

import numpy as np

matrix_1 = np.array([[1,2,3],  
                    [4,5,6],
                    [7,8,9]])

matrix_2 = np.array([[0,1,2],
                    [3,4,5],
                    [6,7,8]])

result = np.dot(matrix_1, matrix_2)

print(result)

# return dot product

res = np.dot(matrix_1,matrix_2)

# print resulting matrix

print(res)
```
## `torch`
```python
import torch

matrix_1 = torch.tensor([[1,2,3],
                        [4,5,6],
                        [7,8,9]])

matrix_2 = torch.tensor([[0,1,2],
                        [3,4,5],
                        [6,7,8]])

product = torch.matmul(matrix_1, matrix_2)

print(product)
```
