# Control Structures and Error Handling

**Learning Objectives:**

* Understand and apply JavaScript control structures to direct the flow of the program.
* Learn to handle errors gracefully in JavaScript applications.

**Conditional Statements:**

* Introduction to `if`, `else if`, `else`, and `switch` statements for decision-making in code.

```javascript
let score = 85;
if (score >= 90) {
  console.log("A grade");
} else if (score >= 80) {
  console.log("B grade");
} else {
  console.log("C grade or below");
}
```

**Loops:**

* Discuss the use of `for`, `while`, and `do...while` loops for repeating actions.

```javascript
// for loop
for (let i = 0; i < 5; i++) {
  console.log(`Iteration ${i}`);
}

// while loop
let i = 0;
while (i < 5) {
  console.log(`Iteration ${i}`);
  i++;
}
```

**Error Handling:**

* Using `try`, `catch`, `finally`, and `throw` to handle errors and exceptions.

```javascript
try {
  // Code that may throw an error
  throw new Error("Something went wrong!");
} catch (error) {
  console.error(error.message);
} finally {
  console.log("This always runs.");
}

```

#### Activities:

#### 1. Conditional Statements: Movie Rating Filter

* **Objective:** Create a function that categorizes movies based on their rating
* **Task:**
  * Write a function that takes an array of movie objects (each movie object has properties: title and rating) and a rating threshold.
  * The function should return an array of movie titles that have a rating equal to or higher than the threshold.
*   **Code Snippet:**

    ```javascript
    const movies = [
      { title: "Inception", rating: 8.8 },
      { title: "The Matrix", rating: 8.7 },
      { title: "Interstellar", rating: 8.6 },
      { title: "The Room", rating: 3.7 }
    ];

    function filterMoviesByRating(movies, threshold) {
      return movies.filter(movie => movie.rating >= threshold).map(movie => movie.title);
    }

    console.log(filterMoviesByRating(movies, 8.5));
    ```

#### 2. Error Handling: Safe Division

* **Objective:** Perform division operations safely, handling any potential errors.
* **Task:**
  * Create a function that takes two numbers as arguments and performs a division operation.
  * If the divisor is 0, throw an error.
  * Use `try...catch` to handle the error and print a friendly message.
*   **Code Snippet:**

    ```javascript
    function safeDivision(dividend, divisor) {
      try {
        if (divisor === 0) throw new Error("Cannot divide by zero.");
        return dividend / divisor;
      } catch (error) {
        console.error(error.message);
        return undefined;
      }
    }

    console.log(safeDivision(10, 0));
    ```

#### 3. Conditional Statements and Loops: Grade Calculator

* **Objective:** Calculate the final grade based on scores.
* **Task:**
  * Write a function that takes an array of scores and calculates the final grade based on the following criteria:
    * 90+ = A
    * 80-89 = B
    * 70-79 = C
    * 60-69 = D
    * Below 60 = F
*   **Code Snippet:**

    ```javascript
    function calculateGrade(scores) {
      let average = scores.reduce((acc, curr) => acc + curr, 0) / scores.length;
      if (average >= 90) return 'A';
      else if (average >= 80) return 'B';
      else if (average >= 70) return 'C';
      else if (average >= 60) return 'D';
      else return 'F';
    }

    console.log(calculateGrade([85, 92, 88]));
    ```







