# HouseCanary PyCon 2016 Coding Challenge

### The Challenge

In the search for great Software Engineers, HouseCanary is hosting a coding challenge for the attendees of PyCon 2016! Any attendee who submits code that passes our public test suite gets a free HouseCanary T-shirt.

This is also an opportunity for job seekers. If you’d like to be considered for a career at HouseCanary, please attach a resume along with your submission. Take a look at our job openings(link) and see if you’re a match.

### Submitting

Using Python 3 and only the standard library, write a function that solves the problem below. The function should be name [something]. It takes a file object as its only argument and returns an int or None.

Copy the function into a secret GitHub Gist(link) and send the link to challenge@housecanary.com. Make sure to include your resume if you’re interested in a career at HouseCanary(link).

After we run the code locally, we’ll send you an email with directions to the HouseCanary booth where you can pick up your prize.

### The Problem

You are given a 2D array of integers 'M'. The value M[x][y] is an
integer corresponding to the number of homes located in row 'x' and column 'y'.
You can assume value of each cell in 'M' is a positive integer <= 100.

Find the largest number of homes inside the 2D array 'M' that
can be contained in a rectangle of size 'a' rows and 'b' columns -- let's call
this the 'search rectangle'. Both a and b are positive integers, and will be
provided per problem instance you are asked to solve.

You can assume that the sum of values in the 2D array 'M' will never be
be bigger than maximum value of an integer in your computer.
Example Problem Instance

Location Array 'M':

    [[0, 3, 1, 6],
    [6, 9, 9, 0],
    [2, 8, 9, 2],
    [8, 8, 8, 5]]    
Each cell value indicates number of homes located in that cell location.

Search rectangle a x b:
    1. a=3, b = 3
    2. a=2, b=2
    3. a=1, b=2

Solution:
    1. Search rectangle of size 3 by 3 with largest number of homes:

    [[6, 9, 9],
    [2, 8, 9],
    [8, 8, 8]]

    Number of homes: 67

    2. Search rectangle of size 2 by 2 with largest number of homes:

    [[9, 9],
     [8, 9]]

    Number of homes: 35

    3. Search rectangle of size 1 by 2 with largest number of homes:

    [[9, 9]]

    Number of homes: 18


### Input File Format

    N
    SEARCH_RECTANGLE_ROWS SEARCH_RECTANGLE_COLUMNS
    NUM_ROWS NUM_COLUMNS
    DATA (NUM_ROWS by NUM_COLUMNS)

First line in input file is the number of problem instances to solve (N).

Second line contains two space separated integers corresponding to number of rows
and columns in the search rectangle.

Third line contains two space separated integers corresponding to number of rows
and columns in location array 'M'.

The next NUM_ROWS lines contain NUM_COLUMNS space separated integers each. These
lines correspond to rows and columns in location array 'M'.



For example, the following contains two problem instances (file inputs/sample.txt):

    3
    2 3
    3 8
    1 2 3 4 80 20 0 5
    5 8 20 0 0 0 0 1
    9 1 1 2 3 5 5 9
    4 5
    4 9
    0 0 2 4 8 2 0 5 1
    1 8 20 5 0 0 0 1 2
    7 1 0 2 3 5 5 9 5
    0 1 1 4 3 5 5 9 0
    20 3
    3 8
    0 2 3 4 80 20 0 5
    1 8 20 0 0 0 0 1
    2 1 1 2 3 5 5 9

### Output format

For each problem instance print an integer equivalent to the
maximum number of homes possible in the search rectangle, followed by a new
line character '\n'. If no solution exists, print the word 'None' (without quotes)
followed by the new line character '\n'.

For the sample input above, the output should be:
    107
    75
    None

## Running the Code
Clone this repo to your machine
Modify the function in [whatever].py to pass the challenge
Run the tests with [unittests command] or the test runner of your choice

Your code will be tested on a [Macbook Details] with vanilla Python 3.5.1. There is a time limit to each test and your code will need to be reasonably efficient (vague?) to pass.

When you’re done, follow the submission guidelines. 

## The Fine Print

Prizes are while supplies last. Contest ends at 5PM on Wednesday June 1st and prizes must be picked up before then. Entrants must be attendees of PyCon 2106.

