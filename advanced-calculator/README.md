# Simple Calculator Project

## Overview
This project is a calculator that allows users to input mathematical expressions using buttons and view the results.

## Features
- **Input Field:** Displays the entered expression.
- **Answer Field:** Shows the calculated result.
- **Buttons:**
  - `C`: Clears the input and result fields.
  - Number buttons (0-9): Input numbers.
  - Operator buttons (`+`, `-`, `*`, `/`): Perform calculations.
  - `=`: Evaluates the expression and displays the result.

```html
<input type="text" id="display" disabled />
<input type="text" id="answer" disabled placeholder="Answer" />
<button onclick="clearDisplay()">C</button>
<button onclick="addToDisplay('+')">+</button>
<button onclick="addToDisplay('-')">-</button>
<button onclick="addToDisplay('*')">*</button>
<button onclick="addToDisplay('/')">/</button>
<button onclick="calculateResult()">=</button>
```

## JavaScript Functions

### `clearDisplay()`
Clears both the input and answer fields, resetting the calculator.

```js
function clearDisplay(){
  display.value = "";
  answer.value = "";
}
```

### `addToDisplay(number)`
Appends the clicked number or operator to the display field.

```js
function addToDisplay(number) {
  display.value = display.value + number;
}
```

### `calculateResult()`
Evaluates the expression entered in the input field and displays the result.

```js
function calculateResult(){
  answer.value = eval(display.value);
}
```

## Usage
1. Click the number buttons to enter a mathematical expression.
2. Click the operator buttons to perform operations.
3. Click the `=` button to evaluate the expression.
4. Click the `C` button to clear the fields and start over.

## Notes
- The project uses the `eval()` function, which should be used with caution to avoid security risks.

