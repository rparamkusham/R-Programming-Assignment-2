# R-Programming-Assignment-2
# The following are the runtime computation commands
# to test the caching of the metrix inversion

> source("RP_Programming_Assignment_2.R")
> 
> x = rbind(c(1, -2), c(-2, 1))
> 
> m = makeCacheMatrix(x)
> 
> m$get()
     [,1] [,2]
[1,]    1   -2
[2,]   -2    1
> 
> cacheSolve(m)
           [,1]       [,2]
[1,] -0.3333333 -0.6666667
[2,] -0.6666667 -0.3333333
> 
> cacheSolve(m)
getting cached data.
           [,1]       [,2]
[1,] -0.3333333 -0.6666667
[2,] -0.6666667 -0.3333333
> 
## End of the file
