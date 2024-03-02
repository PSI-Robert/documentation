# Working with Arrays and Objects

**Learning Objectives:**

* Master the manipulation and iteration of arrays and objects, essential for handling data in JavaScript.
* Understand how to access, modify, and iterate through array and object elements.



* **Arrays:**
  * Overview of arrays, including creation, access, and updating elements.
  *   Introduction to array methods like `map`, `filter`, `reduce`, `forEach`, and `find`.

      ```javascript
      const numbers = [1, 2, 3, 4, 5];
      const doubled = numbers.map(number => number * 2);
      console.log(doubled); // [2, 4, 6, 8, 10]
      ```
* **Objects:**
  * Discuss objects as collections of key-value pairs.
  * Accessing, adding, and modifying properties.
  *   Introduction to `Object.keys()`, `Object.values()`, and `Object.entries()`.

      ```javascript
      const person = {
        name: "Rob",
        age: 30,
        isDeveloper: true
      };
      console.log(Object.keys(person)); // ["name", "age", "isDeveloper"]
      ```

**Activities:**

* **Code-Along:** Demonstrate practical uses of array methods and object manipulation.
  *   Use `filter` to find all even numbers in an array.

      ```javascript
      const evens = numbers.filter(number => number % 2 === 0);
      console.log(evens); // [2, 4]
      ```
  *   Modify an object property and add a new one.

      ```javascript
      person.job = "Backend Developer";
      person.age = 31;
      console.log(person);
      ```

**Afternoon Session: Hands-on Practice**

* **Group Activity:** Assign tasks focusing on creating and manipulating complex data structures.
  * _Exercise Example:_
    *   Create a function that takes an array of objects (representing people) and sorts them by age.

        ```javascript
        const people = [
          { name: "Alice", age: 25 },
          { name: "Bob", age: 30 },
          { name: "Charlie", age: 22 }
        ];

        function sortByAge(people) {
          return people.sort((a, b) => a.age - b.age);
        }

        console.log(sortByAge(people));
        ```
* **Pair Programming:** Work in pairs to tackle exercises that require both arrays and objects.
  * _Project Idea:_
    *   Implement a simple inventory system where items are objects stored in an array. Include functions to add, remove, and search for items by name.

        ```javascript
        javascriptCopy codelet inventory = [
          { name: "apples", quantity: 2 },
          { name: "bananas", quantity: 0 },
          { name: "cherries", quantity: 5 }
        ];

        function addItem(inventory, item) {
          inventory.push(item);
        }

        function findItemByName(inventory, name) {
          return inventory.find(item => item.name === name);
        }

        addItem(inventory, { name: "dates", quantity: 10 });
        console.log(findItemByName(inventory, "dates"));
        ```
