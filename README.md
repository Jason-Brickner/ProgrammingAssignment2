### Testing the functions:
1.  run makeCacheMatrix and cacheSolve functions.
2.  define a square matrix (i.e. x <- matrix(1:4, 2, 2)).
3.  run the makeCacheMatrix function on x and assign the result to i (i.e. i <- makeCacheMatrix(x)).
4.  call i$get() to return the original matrix.
5.  call i$getinv() to return NULL.
6.  run cacheSolve on i to generate the inverse of the matrix (cacheSolve(i)).
7.  call i$getinv() to test if the inverse of the matrix is cached.
8.  rerun cacheSolve on i to retrieve the cached matrix along with the message "getting cached data".
9.  create a new matrix (i.e. y <- matrix(5:8, 2, 2)).
10.  run makeCacheMatrix on y and assign it to the variable g (i.e. g <- makeCacheMatrix(y)).
11.  generate the inverse of y and assign it to c (i.e. c <- solve(y)).
12.  set the cached inverse for g to c (i.e. g$setinv(c)).
13.  run cacheSolve on g to retrieve cached matrix, along with the message "getting cached data" (i.e. cacheSolve(g)).

### Assignment: Caching the Inverse of a Matrix

Matrix inversion is usually a costly computation and there may be some
benefit to caching the inverse of a matrix rather than computing it
repeatedly (there are also alternatives to matrix inversion that we will
not discuss here). Your assignment is to write a pair of functions that
cache the inverse of a matrix.

Write the following functions:

1.  `makeCacheMatrix`: This function creates a special "matrix" object
    that can cache its inverse.
2.  `cacheSolve`: This function computes the inverse of the special
    "matrix" returned by `makeCacheMatrix` above. If the inverse has
    already been calculated (and the matrix has not changed), then
    `cacheSolve` should retrieve the inverse from the cache.

Computing the inverse of a square matrix can be done with the `solve`
function in R. For example, if `X` is a square invertible matrix, then
`solve(X)` returns its inverse.

For this assignment, assume that the matrix supplied is always
invertible.

In order to complete this assignment, you must do the following:

1.  Fork the GitHub repository containing the stub R files at
    [https://github.com/rdpeng/ProgrammingAssignment2](https://github.com/rdpeng/ProgrammingAssignment2)
    to create a copy under your own account.
2.  Clone your forked GitHub repository to your computer so that you can
    edit the files locally on your own machine.
3.  Edit the R file contained in the git repository and place your
    solution in that file (please do not rename the file).
4.  Commit your completed R file into YOUR git repository and push your
    git branch to the GitHub repository under your account.
5.  Submit to Coursera the URL to your GitHub repository that contains
    the completed R code for the assignment.

### Grading

This assignment will be graded via peer assessment.
