# Modules covered in Machine learning fundamentals
* optimization 
* statastical ML 
* probablistic ML
* representation learning 
* deep learning and more 

## plan for the talk 
* basic linear algebra 
* vector calculus 
* probability theory 
* Loss functions in ML

### Linear algebra 
![](Images/2023-05-21-14-46-20.png)

### Euclidian Space: 
> A space in any finite number of dimensions n, in which the points are designated by coordinates (one foreach dimensions) and the distance between two points is given by distance formula.  

### What's coordinates: 
> ordered collection of points from which we can identify the location with some reference points. 
![](Images/2023-05-21-14-54-10.png)

### Distance formula: 
> distances between the pairs of points in terms of coordinates. 
![](Images/2023-05-21-14-56-13.png)

### Euclidian spaces: 
distance formula for n dimensional space ( square root of sum of the squares of all the components of the vector)![](Images/2023-05-21-14-57-31.png)


### valid distance metric: 
dist(A,B) > 0 
dist(A,A) = 0 
dist(A,B) = dist(B,A)
for any points A B and C dist(A,C) < dist(A,b) + dist(B,C)

eg. manhatten distance

## vectors in euclidian space: 
geometric object which has magnitude and direction. 
![](Images/2023-05-21-15-10-43.png)

Magnitude: Length in between two points A and B. Typically the vectors start with the (0,0,..) So AB = B = [b1,b2,b3,...,bn]

### What can we do with the vectors: 
- Linear operations
    - Products
    ![](Images/2023-05-21-15-17-36.png)
- inner product
    scalar which is the sum of the products of the corrosponding components ( the result is scalar)
    - symmetric
    - multiplication on zero 
    - orthogonality of the vectors ( the inner products will be 0) 
    - linearity: scalars can be multiplied inside without affecting the operations by other scalars

    ### Application in ML
    ![](Images/2023-05-21-15-22-26.png)

- component wise products 
multiplication sequentially 
![](Images/2023-05-21-15-23-13.png)

    ### application
    Adam update equation !![](Images/2023-05-21-15-24-32.png)

    we use the component wise product for calculating this.

- kronecker product 
multiplying components as scalar and multipying as full components in vector V
![](Images/2023-05-21-15-25-28.png) 

### Vector norms: 
![](Images/2023-05-21-15-44-57.png)
![](Images/2023-05-21-15-47-57.png)
sparsity norm is not valid norm ( L0 norm ) 

### Linear independence: 
collection of the vectors is called linearly independent if 
multiplication of zero scalar to all the vectors sum results in 0 
and if it's zero then always the scalar is zero

## matrices
![](Images/2023-05-21-16-05-15.png)

### matrix operations 
- transpose: converting the rows into columns of the matrix 
**symmetric** no of rows and columns are same and original matrix and transpose matrix are same
- linear operations : add sub multiply by scalar


## matrix operatinos application machine learning 
**feedforward network:** ![](Images/2023-05-21-19-10-58.png)
feed forward network is another matrix multiplication  