# cit382-assign01
Created with CodeSandbox

For this assignment, you'll be creating a React app that will list a summary of two quiz results. The results will include the name of the quiz, the average score, the maximum score and the student name with the maximum score, and the minimum score and the student name with the minimum score. Below is the sample output:

# Overview

## Requirements

Below are the requirements for this assignment.

#### Quiz Data

Create a file in your src folder called data.js. This file will consist of a single object called quizData. You will need to export the object using the following code:

``` export const quizData = { }; ```

The quizData object has the following format:

```

quizData = {
  term: "",
  quizzes: [
    {
      quizName: "",
      scores: [
        {
          last: "",
          first: "",
          score: 0
        },
      ]
    }
  ]
};

```
#### You will use two websites to generate 10 random names, and 10 random numbers between 0 and 10. Split the results into two groups to represent two separate quizzes. Update your quizData object with the 10 names and scores (five for each quiz).

To generate the random names, use:

https://www.name-generator.org.uk/quick/ (Links to an external site.)

To generate the random integers, use:

https://www.random.org/integers/?num=10&min=1&max=10&col=1&base=10&format=html&rnd=new (Links to an external site.)

You will  need to import the file in App.js using the following code:

``` import { quizData } from "./data.js"; ```

#### Average Function

You will need to create a function called average() with the following signature:

``` average(data) ```

Input: The data parameter is the quizData object.

Output: The average() function will work through the quizData object contents, and return a string array that contains the final output, where each array element is the contents shown in the output above for the quiz results.  Each array element is a string with no JSX.

You must use ```Array.push()``` with a template literal (Links to an external site.) to create the string for each array element.

#### AverageJSX Function

You will need to create a fuction called averageJSX() with the following signature:

```averageJSX(data)```

Input: The data parameter is the output array from the average() function.

Output: The averageJSX() function will return a JSX object that consists of a div for each row in the string array.

You will need to update the ```App()``` function to call both ```average()``` and ```averageJSX()``` functions.

Striped Output

You will need to use CSS to stripe the quiz results rows as shown in the output above. You will need to create two new class selectors, ```QuizRowOdd``` and ```QuizRowEven```, and use the nth-child pseudo-selector and the > descendant selector. You will also need to add the classes into the ```App()``` function to engage the CSS selectors for striping.

#### Documentation and Whitespace

Good use of function and methods, and variable names, promote self-documentation of your code. Regardless, you should still consider adding comments to your code that improves the understanding of how the code works. The documentation can also serve as an outline of how to solve the problem. In general, you should consider adding comments that describe the functionality of blocks of code.

For example, the comments below are my comments from my average() function.

```
// Produce string array of quiz results

// Initialize output array

// Iterate through the quizzes

// Initialize variables

// Iterate through the scores of each quiz

// Extract the quiz score and name

// Accumulate the total score for the current quiz

// Update max and min score and names

// Extract quiz name

// Calculate quiz average

// Use template literal to construct result and push to output array

// Return string array
```
Deliverables

For this assignment you will be uploading your work from Lab 1 and Lab 2 as well as your work from this assignment.

Create a single compressed/zip file of the files from the assignment on this page. The file will contain App.js, data.js, index.js, and styles.css. Name the file assign01.zip.

Important: Do not include the node_modules folder or any GIT folders in your compressed files.

Create a single compressed file that contains all of the assign assignment files from Lab 1, Lab 2, and this assignment page. Name the file cit382-assign01.zip. The file will contain the following files, with their point values in parentheses.

    (5) lab01-sandbox.zip
    (5) lab01-local.zip
    (25) assign01.zip

Use the Assignment 1 Canvas site to submit/upload the compressed/ZIP file.

Once uploaded, revisit the Assignment 1 page in Canvas and confirm the file was uploaded.

Remember, you are responsible to submit your assignments before the deadline. Late submissions will not be accepted.
