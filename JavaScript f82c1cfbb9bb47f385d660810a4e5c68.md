# JavaScript

- **Comment :**
    - **Single line**:
    
    ```jsx
    // Single-line comments start with //
    ```
    
    - **Multi-line**:
    
    ```jsx
    /* Multi-line comments start
     and end with */ 
    ```
    
- **Var:** Variables are containers for storing data (storing data values).
    - They are named storage. We need variables to store data
    - There are two variable scopes in JS
        - Global
        - Local
    - **Const**: If we want a general rule we declare variables with const
    - **Let**: If the value of the variable can or will change, we use let
    
    ```jsx
    const price1 = 5;
    const price2 = 6;
    let total = price1 + price2;
    ```
    
    - Variables are identified by unique names called **identifiers**
        - Those identifiers can contain letters, digits, underscores, and dollar signs
        - Names are case-sensitive (’a’ and ‘A’ are different variables)
    - Declaring happens when we create a variable and we assign value to the variable using ‘=’ this sign
    
    ```jsx
    var firstName
    let firstName
    
    // We've declared a 'firstName' variable
    
    firstName = "Abel"; // Assigning a value to the variable
    
    let firstName = "Abel"; // Assigning value and declaring variable at the same time
    
    let name = "Abel", school = "ACT", age = 21; // Declaring multiple variables at once
    ```
    
- **Let**: A keyword used to define a variable
    - Once variables are defined with this keyword, they cannot be redeclared
    - It must be declared before use
    - The difference they have with the **Const** keyword is that variables declared with const can’t be **reassigned**
    - **Operators**
    
    ```jsx
    let x = 10, y = 20; // Assignment operator
    let z = x + y; // Addition operator
    let z = x * y; // Multiplication operator
    x += 5; // Addition assignment operator
    && // Logical AND
    || // Logical OR
    ! // Logical NOT
    ```
    
- **Data type:** String, Number, Big-int, Boolean, Undefined, Null, Symbol, Object
    - **Object**: Contains an object, an array, and a date
    - **Strings**: Written inside double or single quotes
    - **Numbers**: Written without quotes
    
    ```jsx
    // String
    let text = "John Doe";
    
    // Number
    let x = 3.14;
    let y = 3;
    
    // Big-int
    let x = 999999999999999;
    
    // Boolean
    Boolean(10 > 9)
    
    //Undefined
    let car;    // Value is undefined, type is undefined
    
    // Null
    
    // Symbol
    
    // Object
    ```
    
- **Operators**: Symbols used to assign values, compare values, perform arithmetic operations, and more. Variables are called Operands and an Operator defines the operation.
    - **Arithmetic**
    - **Comparison**
    - **Logical**
    - **Assignment**
    - **Conditional**
    - **String**
    - **Type**
    - **Bitwise**
- **Control flow stat** :
    - **If**: Used to specify a block of code to be executed, if a specified condition is true
    - **Else**: Used to specify a block of code to be executed, if the same condition is false
    - **Else if:** Used to specify a new condition to test, if the first condition is false
    - **Switch:** Used to specify many alternative blocks of code to be executed
- **Loop:** If we want to run the same code over and over again with different results each time we use a loop
    - **For loop:** Loops through a block of code a number of times
    - **Do while:** Loops through a block of code while a specified condition is true
- **Objects:** They are variables that contain many values

```jsx
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

- **Functions:** Fundamental building blocks in JS
    - Set of statements that perform a specific task
    - Executed when it is invoked or called
    
    ```jsx
    function num() {
    	// We have created a new function
    }
    
    num(); // We are calling the function
    
    function num(a, b) {
    	// Function with parameters
    }
    ```
    
    - Local variable: Only accessed from within the function
        - Created when a function starts and deleted when the function is completed
        - Variables with same name can be used in different function
    
    ```jsx
    function myFunction() {
      let carName = "Volvo";
      // code here CAN use carName
    }
    ```
    
- **Arrays:** A special variable, which can hold more than one value
    - They are special types of objects

```jsx
const array_name = ["item1", "item2", "item3", ...]; // Syntax

const array_name = []; // Providing elements after the array is already created
cars[0]= "item1";
cars[1]= "item2";
cars[2]= "item3";

const cars = new Array("Saab", "Volvo", "BMW"); // new keyword creates an array

const cars = ["Saab", "Volvo", "BMW"]; // Accessing full array with JS
document.getElementById("demo").innerHTML = cars;
```

[DOM](https://www.notion.so/DOM-6249e51986ba42478a8a4563f2381b94)

[JSON](https://www.notion.so/JSON-2e409d158af64a84a230047ad35864e1)