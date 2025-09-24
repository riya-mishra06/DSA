

### **JavaScript String Methods Documentation**

---

#### **1. String Length**

* **Definition**: `.length` is a property that returns the number of characters in a string.
* **Example**:

  ```js
  let str = "Hello, world!";
  console.log(str.length);  // Outputs: 13
  ```
* **Important**: Includes spaces, punctuation, and special characters.

---

#### **2. String Concatenation**

* **Using `+` operator**:

  * Combines multiple strings.
  * Example:

    ```js
    let firstName = "John";
    let lastName = "Doe";
    let fullName = firstName + " " + lastName;
    console.log(fullName);  // Outputs: "John Doe"
    ```

* **Using Template Literals (backticks)**:

  * More readable and allows embedding variables inside strings.
  * Example:

    ```js
    let fullName = `${firstName} ${lastName}`;
    console.log(fullName);  // Outputs: "John Doe"
    ```

---

#### **3. `.charAt()` Method**

* **Definition**: `.charAt(index)` returns the character at the given index in a string.

* **Example**:

  ```js
  let str = "Hello";
  console.log(str.charAt(0));  // Outputs: "H"
  console.log(str.charAt(4));  // Outputs: "o"
  ```

* **Important**: Indexing starts at **0**, and it returns an empty string if the index is out of range.

---

#### **4. Palindrome Check with `.charAt()`**

* **Problem**: Check if a string is a palindrome (same forwards and backwards).

* **Solution**:

  * Loop through the string up to the middle.
  * Compare characters from the start and the end.
  * If any pair doesn’t match, it's not a palindrome.

* **Example Code**:

  ```js
  let str = "racecar";
  let pal = true;

  for (let i = 0; i <= str.length / 2; i++) {
      if (str.charAt(i) !== str.charAt(str.length - i - 1)) {
          pal = false;
          break;
      }
  }

  console.log(pal);  // Outputs: true if palindrome, false if not

