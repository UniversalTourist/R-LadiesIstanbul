R For Beginners
========================================================
author: Hazel Kavili
date: 2017-09-30
width: 1400
height: 1280
font-family: 'Helvetica'

R and R Studio
========================================================

Let's meet with the most used IDE (integrated desktop environment) for R

- Source
- Console
- Environment, History, Connections
- Files, Plots, Packages, Help, Viewer

Looking for Help!
========================================================
- Ask Google
- [An introduction to R](http://cran.us.r-project.org/doc/manuals/R-intro.pdf)
- [Try R](http://tryr.codeschool.com)
- R mailing list: first, learn how to ask questions!
- [R Tutorials](http://www.tutorialspoint.com/r/)
- Get help from R:


```r
help.start()
help(mean)
?mean
example(mean)
```


Getting Started 
========================================================

**R commands:**
- are case sensitive
- can be seperated either by a semi-colon(;), or by a newline
- #comment

**Objects:**
- varibables, arrays of numbers, character strings, functions

Getting Started - II
========================================================

**Assignment**  and **Basic Operators**
- use **<-** for assigments
- +,-, *, /, ^, %%

**Logical Operators**
- <,>, <=, >=, ==, !=, !x, x & y, x | y

**Others**
- sum, sqrt, min, max, mean, var, sd, abs, summary

Most Frequently Used Objects
========================================================
- Vectors
- List
- Matrices
- Arrays
- Factors
- Data Frames

Vectors
========================================================
- use **c()** for concatenate more than one element.

```r
books <- c("history", "sci-fi", "fantasy")
print(books)
```

```
[1] "history" "sci-fi"  "fantasy"
```

```r
print(class(books))
```

```
[1] "character"
```



Examples
========================================================

```r
#this is R-Ladies Istanbul
X <- 10
x <- 5
print(paste("X is", X))
```

```
[1] "X is 10"
```

```r
print(paste("x is", x))
```

```
[1] "x is 5"
```

```r
cat("X and x are equal? = ", X == x)
```

```
X and x are equal? =  FALSE
```


```r
myNumbers <- c(1:10) # c is short for concatenate
myNumbers
```

```
 [1]  1  2  3  4  5  6  7  8  9 10
```

```r
rep(myNumbers, times = 3)
```

```
 [1]  1  2  3  4  5  6  7  8  9 10  1  2  3  4  5  6  7  8  9 10  1  2  3
[24]  4  5  6  7  8  9 10
```

```r
twice <- rep(myNumbers, each = 2)
```

Examples - II
========================================================

```r
y <- c(1,2,3,10,15,20)
z <- c(y,4,5,6,y)
print(y)
```

```
[1]  1  2  3 10 15 20
```

- Vector Arithmetic

```r
5/y
```

```
[1] 5.0000000 2.5000000 1.6666667 0.5000000 0.3333333 0.2500000
```

```r
5*y
```

```
[1]   5  10  15  50  75 100
```

```r
y^2
```

```
[1]   1   4   9 100 225 400
```

```r
sqrt(y)
```

```
[1] 1.000000 1.414214 1.732051 3.162278 3.872983 4.472136
```

Simple Manipulations
========================================================


```r
weights <- c(55, 60, 45, 70, 56, 73, 59, 82)
sum(weights)
```

```
[1] 500
```

```r
mean(weights)
```

```
[1] 62.5
```

```r
sd(weights)
```

```
[1] 11.77164
```

```r
var(weights)
```

```
[1] 138.5714
```

```r
length(weights)
```

```
[1] 8
```

Lists
========================================================
- Lists can contain many different types of elements inside.

```r
myList <- list(c(1,2,3), 15, "hello")
print(myList)
```

```
[[1]]
[1] 1 2 3

[[2]]
[1] 15

[[3]]
[1] "hello"
```

- Choose an element from lists

```r
myList[1]
```

```
[[1]]
[1] 1 2 3
```

```r
myList[[1]][2]
```

```
[1] 2
```

```r
myList[2]
```

```
[[1]]
[1] 15
```


Matrices
========================================================
- A matrix is **two-dimensional** recteangular data set.

```r
myMatrix <- matrix(c(1,2,3,4,5,6), nrow = 2, ncol = 3, byrow = TRUE)
print(myMatrix)
```

```
     [,1] [,2] [,3]
[1,]    1    2    3
[2,]    4    5    6
```

- Choose an element from matrices

```r
myMatrix[1,2]
```

```
[1] 2
```

```r
myMatrix[2,]
```

```
[1] 4 5 6
```

```r
myMatrix[,1]
```

```
[1] 1 4
```

Arrays
========================================================
- Arrays can be of nay numbe rof dimensions












