# sqrtn
An R pacakge to calculate sqrt(n) with very high precision. "sqrtn" implements dramatically fast. It takes only less than 30 seconds to approximate sqrt(2) with 100,000 digits.

# Installation

    #install.packages("devtools")
    library(devtools)
    install_github("Tesla-Xiao/sqrtn")

# Usage

   - [x] [sqrtn-manual.pdf](https://github.com/Tesla-Xiao/sqrtn/blob/master/inst/sqrtn-manual.pdf) ---------- Details of the usage of the package.
   
   - [x] [sqrt2.txt](https://github.com/Tesla-Xiao/sqrtn/blob/master/inst/sqrt2.txt) ---------- The first one hundred thousand digits of the square root of 2.

# Example
    library(sqrtn)

    fit <- sqrtn(100)
    print(fit$sqrt2,quote=FALSE)
    #------------------------
    fit <- sqrtn(100,3)
    print(fit$sqrt2,quote=FALSE)
    #------------------------
    fit <- sqrtn2(100,15)
    print(fit$sqrt,quote=FALSE)    
    #------------------------
    fit <- sqrtn2(100,17)
    print(fit$sqrt,quote=FALSE)     

# Development
This R package is developed by Xu Liu (liu.xu@sufe.edu.cn) and Xiao Zhang.
