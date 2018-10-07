# Derivatives-in-R
some example of derivatives in R

#Example

rule8 <- function(x,n){
  return(n*x^(n-1))
}
library(Ryacas)
x <- Sym("x")
Simplify(deriv(x^2,x))

#No 1

rule11 <- function(x){
  return(1/2*sqrt(x))
}
rule11(4)

#No 2

#No 2-1

library(Ryacas)
x <- Sym("x")
Simplify(deriv(2*x^5,x))

#No 2-2

library(Ryacas)
x <- Sym("x")
Simplify(deriv(x^2+4,x))

#No 2 -3

library(Ryacas)
x <- Sym("x")
Simplify(deriv(x^5-6*x^7,x))

