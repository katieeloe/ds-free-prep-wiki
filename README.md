# Data Science Free Prep Wiki
This repo serves as a source for answers to common questions for the data science free prep material.  We hope to have an active community within the prep course channel, however, several questions are sufficiently common that it's a good idea to check here first.  The answers should be organized by section, so please have a look, and if your question is not addressed, feel free to put your question in the slack channel.


## Contents
1. [Intro to Learn](#1-learn)
2. [Intro to Data Science Workflow](#2-Workflow)
3. [Intro to Python](#3-Python-Intro)
4. [Strings and Lists](#4-Strings-and-Lists)
5. [Tuples, Dicts, and Sets](#5-Tuples-Dicts-Sets)
6. [Functions](#6-Functions)
7. [Linear Algebra](#7-Linear-Algebra)
8. [NumPy](#8-NumPy)
9. [SQL](#9-SQL)
10. [Probability](#10-Probability)
11. [Final](#11-Final)


### 1 Learn

### 2 Workflow

### 3 Python Intro

#### 3.4.1 Anaconda Install
```I installed Anaconda on my Mac (OS X) and now when I type "conda --version" or "ipython" it tells me command not found. I can open Anaconda Navigator just fine. Anyone know what's happening?```

The installation for anaconda should add the path to the directory in your unix ```$PATH``` variable.  Typically one of two issues have happened.<br/><br/>
1.) You're in the same terminal window you did the install in.   If this is the case, the PATH variable has not been refreshed because your bash profile has not been rerun.  You can test this in the following way:
```
grep conda ~/.bash_profile
```

You should see output similar to this:
```
# added by Anaconda3 installer
export PATH="/Users/josephgartner/anaconda3/bin:$PATH"
```
If you run the grep command as listed, and you see something similar, then you simply need to execute ```source ~/.bash_profile```


2.)  You chose not to add the path to anaconda to your PATH variable.  If you run the above ```grep``` command and don't see the next two lines, then you didn't have it add anaconda to your path.  You can fix that by doing:
```
echo "export PATH=\"/Users/josephgartner/anaconda3/bin:$PATH\"" >> ~/.bash_profile
source ~/.bash_profile
```

*Note* you'll need to replace /Users/josephgartner/ with whatever the path to your anaconda install is.


### 4 Strings and Lists

### 5 Tuples Dicts Sets

### 6 Functions

### 7 Linear Algebra

### 8 NumPy

### 9 SQL

### 10 Probability

### 11 Final