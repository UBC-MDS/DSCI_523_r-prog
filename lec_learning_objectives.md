## Lecture Learning Objectives
 
### Lecture 1: Reading data, single data frame manipulations & tidying data in R
* Choose and use the appropriate `readr::read_*` function and function arguments to load a given rectangular, plain text data set into R
* Use the assignment symbol, `<-`, to assign values to objects in R and explain how it differs from `=`
* Write a dataframe to a .csv file using `readr::write_csv`
* Use `readr::read_csv` to bring data from standard comma separated value (`.csv`) files into R
* Recall and use the following `dplyr` functions and operators for their intended data wrangling tasks:
    - `select`
    - `filter`
    - `mutate`
    - `%in%`
* Use the pipe operator, `%>%`, to combine two or more functions
* Define the term "tidy data"
* Discuss the advantages and disadvantages of the tidy data format
* Use `tidyr::pivot_wider` & `tidyr::pivot_longer` in R to make untidy data tidy

### Lecture 2: Key datatypes & operators in R
*  Create in R, and define and differentiate in English, the below listed key datatypes in R:
	- logical, numeric, character and factor vectors
	- lists
	- data frames and tibbles
* Use R to determine the type and structure of an object
* Explain the distinction between names and values, and when R will copy an object.
* Use the three subsetting operators, `[[`, `[`, and `$`, to subset single and multiple elements from vectors and data frames
* Compute numeric and boolean values using their respective types and operations
* Write R code that is human readable and follows [the tidyverse style guide](https://style.tidyverse.org/)

### Lecture 3: Working with dates, strings & factors in R
* Manipulate dates and times using the `lubridate` package
* Be able to modify strings in a data frame using regular expressions and the `stringr` package
* Cast categorical columns in a data frame as factors when appropriate, and manipulate factor levels as needed in preparation for data visualisation and statistical analysis

### Lecture 4: Two data frame joins & base R control flow
* Compare and contrast mutating joins, filtering joins and set operations
* Choose the appropriate two table `dplyr` function based on the type of join desired between two data frames, and use it in R to obtained the desired data frame from joining two tables
* Write conditional statements in R with `if`, `else if` and `else` to run different code depending on the input
* Write for loops in R to repeatedly run code

### Lecture 5: Tidy control flow in R
* Explain what a grouped data frame is, and how it can be used
* Use {dplyr}'s `group_by` + `summarize` to perform the split-apply-combine approach in R to iterate over and summarize data by groups
* Identify missing and erroneous values and manage them by removing (via {dplyr}'s `filter`) or replacing (using {dplyr}'s `mutate` + `case_when`)
* Identify where in R code a commonly used functional, a {purrr}'s `map*` function, could be used in place of for loops and write code to do this

### Lecture 6: Functions & testing in R
* In R, define and use a named function that accepts parameters and returns values
* Describe lazy evaluation and `...` (variable arguments) and how it affects functions in R
* explain the importance of scoping and environments in R as they relate to functions
* Use `testthat` to formulate a test case to prove a function design specification
* Use test-driven development principles to define a function that accepts parameters, returns values and passes all tests
* Handle errors gracefully via exception handling
* Use `roxygen2` friendly function documentation to describe parameters, return values, description and example(s).
* Write comments within a function to improve readability
* Evaluate the readability, complexity and performance of a function
* Source and use functions stored as R code in another file, as well as those in R packages/libraries
* Describe what R packages/libraries are, as well as explain when and why they are useful

### Lecture 7: Mapping & nested data frames in R
* Write and use anonymous functions in R in isolation and in combination the functional {purrr} `map`
* Understand the general ideas of the `map*`, `map2*` and `pmap*` variant functions in the {purrr} package and the six types of output options (list, double, integer, logical, character and data frame).
* Create and modify nested data frames using {dplyr} `group_by` + {tidyr} `nest` and {purrr} `map*` functions
* Create unnested data frames using {tidyr} `unnest` 
* Describe situations where nested data frames are useful 

### Lecture 8: Tidy evaluation in R
* Describe data masking as it relates to the `dplyr` functions. Explain the problems it solves for interactive programming and the problems it creates for programming in a non-interactive setting
* Explain what the `enquo()` function and the `!!` operator do in R in the context of data masking as it relates to the `dplyr` functions
* Use the `{{` (read: curly curly) operator (abstracts quote-and-unquote into a single interpolation step), the `:=` (read: walrus) operatpr in R, and `...` (read: pass the dots) to write functions which wrap the `dplyr` functions
