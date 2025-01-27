# JavaScript If Statements and Calculation Functions

## Conditional Statements: `if`, `else if`, and `else`

Conditional statements allow your to program your code to execute based on certain conditions.

### Example 1: `if` and `else`

```js
const age = 18;

if (age == 17) {
  // Execute this code if age is 17
  console.log("Age is 18");
} else {
  console.log("Age is not 18");
}
```

### Example 2: `if`, `else if`, and `else`

```js
const number = 40;

if (number < 5) {
  console.log("40 is greater than 5");
} else if (number == 5) {
  console.log("40 is 5");
} else {
  console.log("All conditions are false");
}
```

---

## Functions to Modify HTML Content

### Example 1: Changing Paragraph Content and Style

```js
function changeParagraph() {
  const paragraph = document.getElementById("paragraph");
  paragraph.innerHTML = "This is a shortened paragraph";
  paragraph.style.backgroundColor = "green";
}

function changeParagraph2() {
  document.getElementById("paragraph").innerHTML = "This is also a button";
  document.getElementById("paragraph").style.backgroundColor = "red";
}
```

---

## Handling User Input with Conditional Statements

You can collect user input from an HTML input field and apply conditional logic.

```js
function typeHereFunction() {
  const typeHere = document.getElementById("type-here").value;
  
  if (typeHere > 10) {
    console.log("Number is greater than 10");
  } else {
    console.log("Number is less than 10");
  }
}
```

---

## Calculation Functions

### Function 1: Displaying User Input

```js
function calculation() {
  let displayScreen = document.getElementById("display-screen");
  let typeHere = document.getElementById("type-here").value;
  
  // Take the value the user types and display it
  displayScreen.value = typeHere;
}
```

### Function 2: Addition Calculator


```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title> Calculator </title>
  </head>
  <body>
    <h1>Addition calculator</h1>

    <input type="number" id="number1" placeholder="0" />
    <input type="number" id="number2" placeholder="1" />
    <input type="number" id="display" placeholder="Ans" />
    <button onclick="additonCalculator()">Calculate</button>
  </body>

  <script src="lesson2.js"></script>
</html>

```

```js
function additionCalculator() {
  let number1 = document.getElementById("number1").value;
  let number2 = document.getElementById("number2").value;

  let display = document.getElementById("display");
  
  // Convert values to numbers and display the sum
  display.value = Number(number1) + Number(number2);
}
```

