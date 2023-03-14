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

### **DOM**

- A different way of representing HTML documents, and we can manipulate the attributes of the objects to modify them
- JS can easily understand the object model hierarchy than the HTML document
- Frames help JS access objects
- JS looks at the objects in terms of nodes. There are 3 types of nodes
    - Element Node: A tag
    - Attribute Node: JS can access the element using the id and perform manipulations
    - Text Node: Content inside the element
- We can access elements of HTML by using the tag name, id, class name
    - **Using tag name:** takes a tag name as a string parameter and returns an object
    
    ```jsx
    document.getElementsByTagName('tagName') // Syntax
    ```
    
    - **Using class name:** Returns an HTML collection object
    
    ```jsx
    document.getElementsByClassName('className') // Syntax
    ```
    
    - **Using an id**: Targets a single HTML element
    
    ```jsx
    document.getElementById('id') // Syntax
    ```
    
- Adding attribute

```jsx
const titles = document.querySelectorAll('h1')
titles[3].className = 'title' // Added a class attribute to the 4th title
titles[3].id = 'fourth-title' // Added an id attribute to the 4th title
titles[5].setAttribute('class', 'title') // Adding attribute using setAttribute()
titles[5].setAttribute('id', 'fourth-title') // Adding attribute using setAttribute()
titles[3].classList.remove('title', 'header-title') // Removing a class
titles[3].classList.add('title', 'header-title') // Appending classes, not over-ride
```

- Adding text
    - textContent is meant to add text to an HTML element, however, innerHTML can add a text or HTML element or elements as a child
    
    ```jsx
    const titles = document.querySelectorAll('h1')
    titles[3].textContent = 'Fourth Title' // Using textContent property
    ```
    
- Adding style

```jsx
const titles = document.querySelectorAll('h1')
titles.forEach((title, i) => {
  title.style.fontSize = '24px' // All titles will have 24px font size
  if (i % 2 === 0) {
    title.style.color = 'green' // If the index is even, color will be green
  } else {
    title.style.color = 'red' // Else the color will be red
  }
})
```

### **JSON**

- Stands for JavaScript Object Notation
- The format is text or string only
- Mostly used when data is sent from a server to a client
- The main difference that has with an object is that we use double quotation here
    - JSON.parse(): a method, to **convert** from JSON to an object
    
    ```jsx
    JSON.parse(json[, reviver])
    ```
    
    - JSON.stringify(): a method, to **convert** the object to JSON
    
    ```jsx
    JSON.stringify(obj, replacer, space)
    /* These two are optional parameters
    	 Replacer: Used as filter
    	 Space: Used as indentations
    */
    ```
    
    ### **Session Storage & Local Storage**
    
    - **sessionStorage**: Only available within the browser tab or window session
        - Designed to store data in a single web page session
        - If the window is closed the session data will be removed
    - **localStorage**: Used to store data on the browser with no expiration data
        - Data will be available on the browser even after the browser is closed
        - Is kept even between browser sessions
        - While storing an array, the object must be stringify’d first
        
        ```jsx
        localStorage.setItem('key', 'value') // Syntax
        localStorage.setItem('firstName', 'Abel') // Storing a string in localStorage
        console.log(localStorage)
        localStorage.getItem('key') // Getting data from localStorage
        localStorage.clear() // Clearing everything stored inside localStorage
        ```
        
        ### **Event Listeners**
        
        - Can be added to any DOM object
        - addEventListener() method takes 2 arguments, an event listener and a callback function
        - Common events are onclick, onchange, onmouseover, onkeyup, onload…
        
        ```jsx
        
        selectedElement.addEventListener('eventlistner', function(e) {
          // The activity you want to occur after the event will be in here
        })
        // or
        selectedElement.addEventListener('eventlistner', e => {
          // The activity you want to occur after the event will be in here
        })
        ```
        
        - List of events:
            - click - when the element clicked
            - dblclick - when the element double clicked
            - mouseenter - when the mouse point enter to the element
            - mouseleave - when the mouse pointer leave the element
            - mousemove - when the mouse pointer move on the element
            - mouseover - when the mouse pointer move on the element
            - mouseout -when the mouse pointer out from the element
            - input -when value enter to input field
            - change -when value change on input field
            - blur -when the element is not focused
            - keydown - when a key is down
            - keyup - when a key is up
            - keypress - when we press any key
            - onload - when the browser has finished loading a page