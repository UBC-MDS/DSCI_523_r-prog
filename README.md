# DSCI 523: Programming for Data Manipulation

Program design and data manipulation using industry-standard software tools designed for statistical work. Organizing, filtering, sorting, grouping, reformatting, converting, and cleaning data to prepare it for further analysis. This course is not eligible for Credit/D/Fail grading.

**Course Webpage** <https://pages.github.ubc.ca/MDS-2020-21/DSCI_523_r-prog_students/README.html>

**Course GitHub repo** <https://github.ubc.ca/MDS-2020-21/DSCI_523_r-prog_students>

**Slack channel:** <https://ubc-mds.slack.com/archives/523_r-prog>  

## Course Learning Outcomes

By the end of the course, students are expected to be able to:
 
1. Read data into R from vanilla (e.g., `.csv`) and non-standard plain text files, as well as common spreadsheet file types (e.g., `.xls`).

1. Manipulate a single data table in R, to do things such as:
    - filtering rows based on a criterion or combination of criteria;
    - selecting variables;
    - creating new variables and modifying pre-existing ones;
    - rearranging the observations or variables in a deliberate way (e.g., sorting).

1. Define tidy data and explain why it is an optimal format for data analysis involving rectangular data in R.

1. Transform data into the tidy data format in R using `tidyr`. 

1. Understand the key data structures in R.

1. Compare and contrast these relationships to the relationship between `vectors` and `data.frame` objects in R. Move data fluidly between these object types.

1. Manage and manipulate data with dates and times, missing values and categorical variables in R. Rename data frame columns.

1. Work with more than one table (as either separate or nested data structures) in R.

1. Translate fundamental programming concepts such as loops and conditionals into R code.

1. Use the split-apply-combine approach in R to iterate over and summarize data by groups.

1. Understand how to write functions in R, document them correctly and assess if they are correct via unit testing.

1. Know when and how to abstract code (e.g., into functions) to make it more modular and robust.

1. Use a functional programming style as another means of code abstraction in R.

1. Use metaprogramming (in particular, tidy evaluation) to make use of tidyverse functions inside custom written functions in R.

1. Produce human-readable code that incorporates best practices of programming and coding style.


## Lecture Schedule

We will be employing a lot of active learning in this course, as you learn programming best by doing! Typically there will be assigned readings & videos that should be reviewed before each lecture. During lecture, we will work in small breakout groups on a lecture worksheet (a Jupyter notebook) that allow us to practice what was covered in the assigned readings & videos. One exception to this is the very first lecture, where I will give a synchronous lecture in the first half of class (as you won't have time to watch a video before this first class given the holiday). This synchronous class will be recorded and shared afterwards.

|   Lecture  | Topic | Required readings | Required videos | Supplementary resources |
|------------|------|-----|------|-----|
| 1 | Reading data, single data frame manipulations & tidying data in R | <ul>[Introduction to Data Science](https://ubc-dsci.github.io/introduction-to-datascience/)<li>[chapter 1](https://ubc-dsci.github.io/introduction-to-datascience/)</li><li>[chapter 2, sections 2.0-2.5 inclusive](https://ubc-dsci.github.io/introduction-to-datascience/reading.html)</li><li>[chapter 3, sections 3.0-3.5 inclusive](https://ubc-dsci.github.io/introduction-to-datascience/wrangling.html)</li></ul> | Video posted to Canvas | <ul><li>[Data Import Cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/data-import.pdf)</li><li>[Data transformation cheat sheet](https://github.com/rstudio/cheatsheets/raw/master/data-transformation.pdf)</li><li>[STAT 545 (chapter 5)](https://stat545.com/basic-data-care.html)</li><li>[Relevant chapters of R for Data Science](https://r4ds.had.co.nz/)</li></ul> |
| 2 | Key datatypes & operators in R | Not applicable | Video posted to Canvas | <ul><li>[Base R cheat sheet](https://rstudio.com/wp-content/uploads/2016/10/r-cheat-sheet-3.pdf)</li><li>[Advanced R (chapters 2-5)](https://adv-r.hadley.nz/)</li></ul> |
| 3 | Working with dates, strings & factors in R | [STAT 545 (Data Analysis 2 section)](https://stat545.com/factors-boss.html) | Video posted to Canvas | <ul><li>[Dates and Times Cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/lubridate.pdf)</li><li>[Work with Strings Cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/strings.pdf)</li><li>[Factors with forcats Cheatsheet](https://github.com/rstudio/cheatsheets/raw/master/factors.pdf)</ul> | 
| 4 | Two table joins & base R control flow | [STAT 545 (Chapter 15) ](https://stat545.com/join-cheatsheet.html) | Video posted to Canvas | [R for Data Science (chapter 13)](https://r4ds.had.co.nz/relational-data.html) |
| 5 | Tidy control flow in R | [STAT 545 (section 7.8)](https://stat545.com/dplyr-single.html#group_by-is-a-mighty-weapon) | Video posted to Canvas | <ul><li>[R for Data Science (section 5.6)](https://r4ds.had.co.nz/transform.html#grouped-summaries-with-summarise)</li></ul> |
| 6 | Functions & testing in R | [R for Data Science (chapter 19)](https://r4ds.had.co.nz/functions.html) | Video posted to Canvas | <ul><li>[ Chapters 6 - 8 of Advanced R](https://adv-r.hadley.nz/functions.html) </li><li>[Testing chapter of R packages](https://r-pkgs.org/tests.html)</li></ul> |
| 7 | Mapping & nested data frames in R | | Video posted to Canvas | <ul><li> [RStudio Apply/map functions Cheat Sheet](https://github.com/rstudio/cheatsheets/raw/master/purrr.pdf)</li><li>[R for Data Science (section 21.5)](https://r4ds.had.co.nz/iteration.html#the-map-functions)</li><li>[R for Data Science (section 25.3 - 25.5)](https://r4ds.had.co.nz/many-models.html#list-columns-1)</li><li>[Advanced R (chapter 9)](https://adv-r.hadley.nz/fp.html)</li></ul>  |
| 8 | Tidy evaluation in R | [Programming with dplyr](https://dplyr.tidyverse.org/articles/programming.html) | Video posted to Canvas | <ul><li>[RStudio Tidy Evaluation Cheat Sheet](https://github.com/rstudio/cheatsheets/raw/master/tidyeval.pdf)</li><li>[Advanced R (Metaprogramming section)](https://adv-r.hadley.nz/metaprogramming.html) |

See the [lecture learning objectives](lec_learning_objectives.md) for a detailed breakdown of lecture-by-lecture learning objectives.  

## Deliverables

You are responsible for the following deliverables, which will determine your course grade:

| Assessment       | Weight  | Due Date         |
| :---:            | :---:   |:---:            |
| Lab 1 | 13%     | 2020-09-13 18:00 PT |
| Lab 2 | 13%     | 2020-09-19 18:00 PT |
| Lab 3 | 13%     | 2020-09-26 18:00 PT |
| Lab 4 | 13%     | 2020-10-03 18:00 PT |
| Worksheet 1 | 1%     | 2020-09-13 18:00 PT |
| Worksheet 2 | 1%     | 2020-09-13 18:00 PT |
| Worksheet 3 | 1%     | 2020-09-19 18:00 PT |
| Worksheet 4 | 1%     | 2020-09-19 18:00 PT |
| Worksheet 5 | 1%     | 2020-09-26 18:00 PT |
| Worksheet 6 | 1%     | 2020-09-26 18:00 PT |
| Worksheet 7 | 1%     | 2020-10-03 18:00 PT |
| Worksheet 8 | 1%     | 2020-10-03 18:00 PT |
| Quiz 1           | 20%     | 2020-09-23 08:00 PT or 21:00 PT |
| Quiz 2           | 20%     | 2020-10-07 08:00 PT or 20:00 PT |

## Class Schedule & office hours

See [calendar](https://ubc-mds.github.io/calendar/).

## Policies

Please see the general [MDS policies](https://ubc-mds.github.io/policies/).

## Dealing With COVID-19

The [COVID-19 pandemic](https://www.who.int/emergencies/diseases/novel-coronavirus-2019/events-as-they-happen) has affected us all in different ways: it's okay to not be okay, and we all need to support each other during this time. With that said:

- My (virtual) door is always open, please feel free to talk to me about how you're doing and if/how I can help you (and if I can't help you, I can point you in the direction of someone who can);
- You don't ever need to explain yourself; if you need support, need to miss a class, or need extra time for an assignment, just ask;
- UBC has [great student support resources](https://students.ubc.ca/covid19) related to COVID-19 (and otherwise).

Further, teaching/learning an intense graduate course like MDS online is a very new concept to all of us. If you have feedback on how I can improve the teaching experience, don't hesitate to reach out - I'm sure things won't be perfect from the get-go.

Finally, here is an official statement from UBC regarding the online learning experience:

>*During this pandemic, the shift to online learning has greatly altered teaching and studying at UBC, including changes to health and safety considerations. Keep in mind that some UBC courses might cover topics that are censored or considered illegal by non-Canadian governments. This may include, but is not limited to, human rights, representative government, defamation, obscenity, gender or sexuality, and historical or current geopolitical controversies. If you are a student living abroad, you will be subject to the laws of your local jurisdiction, and your local authorities might limit your access to course material or take punitive action against you. UBC is strongly committed to academic freedom, but has no control over foreign authorities (please visit http://www.calendar.ubc.ca/vancouver/index.cfm?tree=3,33,86,0 for an articulation of the values of the University conveyed in the Senate Statement on Academic Freedom). Thus, we recognize that students will have legitimate reason to exercise caution in studying certain subjects. If you have concerns regarding your personal situation, consider postponing taking a course with manifest risks, until you are back on campus or reach out to your academic advisor to find substitute courses. For further information and support, please visit: http://academic.ubc.ca/support-resources/freedom-expression.*
