# DSCI 523: Data Wrangling

Converting data from the form in which it is collected to the form needed for analysis. How to clean, filter, arrange, aggregate, and transform diverse data types, e.g. strings, numbers, and date-times.

**Course Webpage** <https://github.ubc.ca/MDS-2018-19/DSCI_523_data-wrangling_students>

**Slack channel:** <https://ubc-mds.slack.com/archives/523_data-wrangling>  

## Course Learning Outcomes

By the end of the course, students are expected to be able to:

  1. Manipulate a single data table like: 
      
      1.1 filtering rows based on a criterion or combination of criteria; 
      
      1.2 selecting variables; rearranging the observations or variables in a deliberate way (e.g., sorting, grouping); 
      
      1.3 creating new variables from one or more existing variables; 
      
      1.4 reshaping data; 
      
      1.5 computing summaries on groups of observations based on one or more categorical variables.
  
  1. Use regular expressions to handle strings;
  
  1. Deal with dates and times; 

  1. Work with more than one table 
  
  1. Detect and handle duplicates and outliers.

  1. Determine appropriate manipulations for two-table data, including lookups and joins with suitably-selected columns.

## Class Meetings

This course occurs in **Block 2** in the 2018/19 school year.  
**Lectures:** Tuesday and Thursday, 11:00-12:30, in [DMP 301](https://goo.gl/maps/P3eSZWYtkuE2)  
**Labs:** Thursday, 13:30-15:30

* Section 1: FNH 50
* Section 2: PCOH 1001
* Section 3: SWNG 305

## Teaching Team

| Position           | Name    | Slack Handle | GHE Handle | Office hours |
| :----------------: | :-----: | :----------: | :--------: | :----------: |
| Lecture Instructor | Jenny Bryan | `@jenny` | `@jennybc`  | Thurs 10/11 & 10/18<br>12:30pm (after class)<br>ICCS/CS room 246|
| Lab Instructor     | Rodolfo | `@lourenzutti` | `@lourenzu` | **To check** | 
| Teaching Assistant | Clement Fung | `@Clement Fung`| `@cfung1 ` | 16:00-17:00 on Wednesday in ESB 1043 |
| Teaching Assistant | Aaron Berk   | `@aberk`| `@aberk` | 12:30-13:30 on Thursday in LSK 311|
| Teaching Assistant | Katie Florko | `@Katie Florko`| `@kflork` | 13:00-14:00 on Tuesday in ESB 3167|

*note - Attendance at office hours is optional* 

## Lectures

*Expect rolling updates as we move through this material in 2018. For example, the lecture on Python is new, so that will cause a bit of reshuffling in elsewhere, as we make room. However, no major content changes are planned*

|   Lecture  | Date | Day | Topic | Readings
|------------|------|-----|-------|---------|
| 1 | 2018-10-09 | Tues | Basic R workflow.<br>Get to know a single data frame or, usually, tibble.<br>Manipulate it: filter rows, select variables, arrange rows, and mutate variables. | [bit.ly/jenny-live-code](http://bit.ly/jenny-live-code)<br>Workflow chapters of [What They Forgot](https://whattheyforgot.org)<br>The [tidyverse](https://www.tidyverse.org) meta-package. See [The tidy tools manifesto](https://cran.r-project.org/web/packages/tidyverse/vignettes/manifesto.html) for a rationale.<br>[Basic care and feeding of data in R](http://stat545.com/block006_care-feeding-data.html)<br>[Introduction to dplyr](http://stat545.com/block009_dplyr-intro.html)<br>[dplyr functions for a single dataset](http://stat545.com/block010_dplyr-end-single-table.html)<br>Slides on [the pipe operator `%>%`](https://speakerdeck.com/jennybc/the-pipe-operator)<br>Slides re: a  [very simple view of some R objects](https://speakerdeck.com/jennybc/simple-view-of-r-objects)<br>[Data transformation](http://r4ds.had.co.nz/transform.html) chapter in [R for Data Science](http://r4ds.had.co.nz/index.html) |
| 2 | 2018-10-11 | Thurs | Create groups in a single data table. Grouped summarisation, window functions, mutation.| Revisit `filter()`, `select()` from [Introduction to dplyr](http://stat545.com/block009_dplyr-intro.html)<br>Resume [dplyr functions for a single dataset](http://stat545.com/block010_dplyr-end-single-table.html) around `rename()`<br> Bonus content if time allows: [reprex](https://github.com/tidyverse/reprex) |
| 3 | 2018-10-16 | Tues |  Tidy data, e.g. reshaping, separating, uniting, and completing variables.| [tidyr](https://tidyr.tidyverse.org) package, a core package of the [tidyverse](https://github.com/tidyverse/tidyverse) meta-package<br>Intro from my [Data Rectangling talk](https://speakerdeck.com/jennybc/data-rectangling)<br>[Tidy data slides](https://github.com/rstudio-education/master-the-tidyverse/blob/master/03-Tidy-Data.pdf) from RStudio's Master the Tidyverse workshop<br>[03-Tidy-Data.Rmd](https://github.com/rstudio-education/master-the-tidyverse/blob/master/exercises/03-Tidy-Data.Rmd) mentioned in the slides<br>[Tidying some Lord of the Rings Data](https://github.com/jennybc/lotr-tidy)<br>[Tidy data](http://r4ds.had.co.nz/tidy-data.html) chapter of R for Data Science<br>[Tidy Animated Verbs](https://github.com/gadenbuie/tidyexplain)<br>[tidyr-spread-gather.gif](https://github.com/gadenbuie/tidyexplain/blob/master/images/tidyr-spread-gather.gif)
| 4 | 2018-10-23 | Thurs | Handling variables of specific type: character data, regular expressions. | [Character vectors](http://stat545.com/block028_character-data.html) |
| 5 | 2018-10-18 | Tues | Working with two tables: join and lookup. | [When one tibble is not enough](http://stat545.com/block033_working-with-two-tables.html)<br>[dplyr joins](http://stat545.com/bit001_dplyr-cheatsheet.html)<br>[table look up](http://stat545.com/bit008_lookup.html)<br>[Relational data chapter](http://r4ds.had.co.nz/relational-data.html) in [R for Data Science](http://r4ds.had.co.nz) |
| 6 | 2018-10-25 | Thurs | Handling variables of specific type: character data, factors, datetimes<br>File I/O | Regex tips re: groups: examples on [rematch2 README](https://github.com/mangothecat/rematch2#readme)<br>[My re-implementation in R](http://stat545.com/block032_character-encoding.html) of [this Ruby post](http://www.justinweiss.com/articles/3-steps-to-fix-encoding-problems-in-ruby/)<br>[ Unicode character inspector](https://apps.timwhitlock.info/unicode/inspect)<br>[String Encoding and R](http://kevinushey.github.io/blog/2018/02/21/string-encoding-and-r/), Ushey blog post<br>[Example of an encoding chart](https://en.wikipedia.org/wiki/Windows-1252)<br>[Be the boss of your factors with forcats](http://stat545.com/block029_factors.html)<br>[Getting data out of and into a file](http://stat545.com/block026_file-out-in.html)<br>[Dates and date-times (mostly awareness-building)](http://stat545.com/block030_date-times.html)<br>Date and date-time coverage in R for Data Science:<ul><li>[Dates and times chapter](http://r4ds.had.co.nz/dates-and-times.html)</li><li>[Dates, date-times, and times](http://r4ds.had.co.nz/data-import.html#parsing-a-vector#Dates-date-times-and-times) subsection in [Data import chapter](http://r4ds.had.co.nz/data-import.html)</li></ul> |
| 7 | 2018-10-30 | Tues | Using the purrr package to work with lists and iterate | [Workshop slides](https://speakerdeck.com/jennybc/purrr-workshop)<br>[My purrr tutorial website](https://jennybc.github.io/purrr-tutorial/index.html)<br>[Row-oriented workflows in R](https://github.com/jennybc/row-oriented-workflows#readme)<br>[How to work with list-columns (webinar)](https://resources.rstudio.com/webinars/how-to-work-with-list-columns-garrett-grolemund)<br>[Many model chapter of R4DS](https://r4ds.had.co.nz/many-models.html) |
| 8 | 2018-11-01 | Thurs | Introduction to data wrangling in Python with `numpy` and `pandas` (guest lecture by Mike Gelbart & Tiffany Timbers) | TBD |

## Live code from class

`.R` files and rendered `.md` from our class meetings will accumulate here:

  * [live-code-from-class](live-code-from-class)

## Labs

|     | Lab topic   | Due Date |
|-----|-------------|----------|
| [1](labs/lab01/lab1.Rmd) | Using `dplyr` to manipulate a single data frame. | 2018-10-13 |
| [2](labs/lab02/lab2.Rmd) | Tidying up messy dataset using `tidyr`, `stringr` and regular expressions. | 2018-10-20 |
| [3](labs/lab03/lab3.Rmd) | Using `forcats` do deal with factors and explore some of relation database functions, such as, `join` and `merge`. Dealing with date using `lubridate` | 2018-10-27 |
| [4](labs/lab04/lab4.Rmd) | Introduction to data wrangling in Python with `numpy` and `pandas` | 2018-11-03 |

## Quizzes
|     | Time | Date | Location |
|-----|------|------|----------|
|  1  | 13:30-14:00 | 2018-10-25 | In your lab |
|  2  | 13:30-14:00 | 2018-11-08 | TBD |

## Reference Material

  * [STAT 545](http://stat545.com/index.html) lessons on data wrangling with the tidyverse in R
    - [Basic care and feeding of data in R](http://stat545.com/block006_care-feeding-data.html)
    - [Introduction to dplyr](http://stat545.com/block009_dplyr-intro.html)
    - [`dplyr` functions for a single dataset](http://stat545.com/block010_dplyr-end-single-table.html)
    - [Cheatsheet](http://stat545.com/bit001_dplyr-cheatsheet.html) for `dplyr` join functions
    - *material to come on tidying*
  * [STAT 545](http://stat545.com/index.html) lessons on specific vector types
    - [Be the boss of your factors](http://stat545.com/block014_factors.html) *to be refreshed with the new forcats package*
    - Regular expression lessons from [2015](http://stat545.com/block027_regular-expressions.html) and [2014](http://stat545.com/block022_regular-expression.html)
  * [purrr tutorial and worked examples](https://jennybc.github.io/purrr-tutorial/index.html) by Jenny Bryan
  * [Using purrr with dplyr](http://lionel-.github.io/2015/10/08/using-purrr-with-dplyr/)
  * [Data Wrangling with Python: Tips and Tools to Make Your Life Easier](http://www.amazon.com/Data-Wrangling-Python-Tools-Easier/dp/1491948817/)
  * [Collection of Python Pandas tutorials](http://pandas.pydata.org/pandas-docs/stable/tutorials.html)
  * [Fun international movie database Pandas data wrangling/exploratory data analysis tutorial](https://github.com/brandon-rhodes/pycon-pandas-tutorial)
