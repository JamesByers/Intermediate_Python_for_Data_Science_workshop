##### Python for Data Science workshop
### Why Python?

### Welcome to Python

**The coding language we'll be using is [Python](https://www.python.org/)**

Python is a free, object-oriented programming language used in a wide variety of development contexts.

Python's focus is on being “friendly,” meaning it simplifies syntax and makes use of white space — like indentations — to promote code readability.

As an open-source programming language, Python is constantly developing and being expanded by programmers across the world. "Open source" means that it's free and people can contribute directly to the main code, so the language is always growing and evolving.

----------------------------------

### By the end of this lesson you will be able to:

+ Describe differences inversions 2.7 vs 3.6.
+ List some examples of Python in the industry.
+ Discuss common languages in data science (e.g., R, Scala) and understand that statistics is language-agnostic.
+ Compare Python to other languages and emphasize specific benefits, e.g., speed, library frameworks, and data pipelines.

----------------------------------

### A (Very) Brief History of Python

Python was originally developed in the late '80s and early '90s as a successor to the previously popular ABC programming language. The creator, Guido van Rossum, built it because ABC was not very adaptable or "extensible," and therefore hard to modify for new use cases. Its major innovation at release was exception handling, or a way to navigate around errors in code. The first version was released in 1991.

Python has gone through many new versions, adding features and functionality along the way. The version primarily used today is Python 2.7, which was released in 2009 alongside Python 3.1.

It might seem odd to release those two versions together, but the distinction between Python 2 and 3 is actually a fairly important one in this conversation.

----------------------------------

### Python 2 vs Python 3

Despite Python 3.0 being released back in 2008, Python 2.7 has persisted as the most commonly used version. There are several reasons for this:
- Python 3 is *not* backwards-compatible, which means it has a lot of trouble reading files written in Python 2. Because so much existing software and other code is written in that language, many programmers have stuck with the older version rather than rewrite all of that code.
- Python 2.7 is still being supported, and will continue to be until 2020. Even at that point, since it is open source, many people are likely to continue developing 2.7.
- Many of the changes in Python 3 make it more efficient, but are less visible on the surface to the user. In fact, the ones that are visible (like changing the "print" statement syntax to require parentheses), are often more irritating to adapt to than they are helpful.

Python 3 is a very capable programming language, and does have advantages over 2.7. Whether or not those advantages outweigh the disadvantages is yet to be seen. In the meantime, you'll likely encounter both versions at some point in your data science journey.

We will be using Python 2.7 as is typical for many companies and cources, as some of the libraries we use throughout cources are not as stable in the current python 3 version as they are in 2.7 .

----------------------------------

### Industry Context

- Python is used in a huge variety of contexts: developing tools, automating processes, performing mathematical calculations, visualizing data analysis, creating websites, and more.

- Python is often ranked as one of, if not the most popular of the coding languages, in large part due to its versatility. Because of its open-source nature, developers are able to create libraries that apply Python to contexts from statistical analysis (SciKit-Learn, StatsModels), to web design (Django, Flask), to software development (ArcGIS and Maya software both incorporate custom Python code, and games like Civilization IV are built on Python frameworks).

- Even when narrowing the focus to data science tasks, it’s difficult to encapsulate the breadth of Python’s applications. Python is used to collect data from sources like databases and APIs; clean and organize that data; and build, tune, and evaluate machine learning models.

- Python has many libraries to assist with these functions, including:
  - **Pandas** is a library that allows for the cleaning, organization, and structuring of data. Think of this as a really agile Excel for use within Python.
  - **SciKitLearn** includes a huge variety of statistical and machine learning models, allowing data scientists to try multiple models on their datasets without the massive time commitment of building these independently.
  - **Tensorflow** is growing in popularity as neural networks become more widespread and broadly utilized. There are increasingly few areas of coding in which Python would not be a very valid choice as the chief programming language.
  - **NumPy** and **StatsModels** allow for advanced mathematical calculations and statistical analysis.

With so many functions, Python can be (and often is) used in virtually every industry context that involves code.
<!--
----------------------------------

_Slide Title_: Python Use Case: Dropbox

_Slide Content_:

Dropbox, the familiar file storage and sharing utility, is built almost entirely on Python. In fact, at PyCon in 2011, engineer Rian Hunter said that 99.9% of Dropbox’s code is written in Python. This includes everything from the server back-end, to the desktop client, to its data analytics. At the same conference, Hunter noted that Dropbox saves 1 million files every 15 minutes, which was more than tweets per minute at the time.

Because the entire stack is in Python, Dropbox data scientists can easily integrate information and perform analytics on large-scale network collaboration. Some examples of analytics performed include account prospecting and prioritization, managing sales-opportunity scores, and building a recommendation engine to help customers understand the best ways to use the software.  
-->

----------------------------------

### Python Is Not Alone

**Python is not the only programming language that can be used for statistics and data science, since the field is language-agnostic. That means that statistics exists on its own, but programming languages allow us to access its methods and information.**
Some other languages include:
- R
- Scala
- C and C++
- Java
- MatLab
- Julia

There are also programs, like SAS and SPSS, that operate as competitors in this space.

This graph from [Fossbytes](https://fossbytes.com/popular-top-programming-languages-machine-learning-data-science/) shows the popularity of various programming languages in job postings in the last several years.

![alt text](assets/programminglanguagespopularity.png)

----------------------------------

### Python's Competitors

#### R
After Python, R is the next frontrunner for the "official language of data science." The free, open-source language is extremely popular, and there's a large community of developers building software around it. R is very adept at working with complex datasets and statistical analysis, however, its usage can be a bit clunky and it's not very easy to work with. While it does have great visualization capabilities in libraries like[R Shiny](https://shiny.rstudio.com/), it isn't often used all the way through development to create a final product. 

### SQL
SQL is not a competitor to Python, since it is a query language and not an entire programming language. It's not an either/or decision between these two. But it's on this list because in terms of database structure, administration, and mining, SQL is an essential tool for the fully capable data scientist.

#### Java
This is the language that often takes over for R in building a system or large framework. It's not great at visualization or statistical modeling, but is very scaleable and can be built on top of if used as a project's base. It's also the basis of tools like Hadoop and Hive, which are used for heftier processing needs.

----------------------------------

### Python's Competitors (Continued)

#### Scala
Based on Java, this is an increasingly popular language, especially for large-scale machine learning. It also incorporates JavaScript, so it's a combination of functional and object-oriented programming. One of Scala's benefits is the ability to work with real-time data, since the technologies that work with streaming data (like Spark) are built on Java as well.

#### Matlab
MatLab is an older language that's far from free. It has a strong foothold in areas like research and academic-based institutions, and is very popular within niche fields like image recognition and signal processing.

#### Julia
Julia is a newcomer to the field, but it's reputed to be a potential competitor to R and Python. It's very fast and expressive, and doesn't have a steep learning curve. It's likely one you'll be hearing about in the field.


----------------------------------

## So, Why Python?

There are many programming languages out there that are used commonly in data science and could be seen as competitors to Python. 

#### The reasons we're using Python (and 2.7 specifically) are:
- **Stable** language, with support from a core source and a thriving community built around it.
- **Versatile**, given the number of libraries developed for it.
- **Friendly**, in that it's both easy to learn and easy to understand/interpret, because of its clean formatting.
- **Powerful**, and can handle complex problems in simple, efficient ways, like by building pipelines within the code.
- **free**!
- **evolving** by virtue of being open source, so it can keep up with the developing data science field.

----------------------------------

## Why Is Python particularly Useful for Data Science?

+ **Open source** - You are not locked into using a particular company's products.
+ **Large community** - Easily find answers to questions.
+ **Interpreted** - Code can be run piece by piece, without creating an executable file.
+ **Abundance of third-party packages** - Prewritten Python packages can be used for data science, video games, website backends, computer vision, and more.
+ **Easy C integration.** - Speed-critical routines can be written in the low-level language C and easily integrated.

Python is an essential tool for your data science capabilities, so have fun exploring it and learning to use it.

----------------------------------
