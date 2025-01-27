# Simple Calculator Project

## Overview
This is a simple calculator that allows users to input mathematical expressions and view the results.

## Features
- **Input Field:** Allows users to enter expressions.
- **Answer Field:** Displays the calculated result.
- **Buttons:**
  - `Clr`: Clears the input and result fields.
  - `=`: Evaluates the expression and shows the result.

```html
<input type="text" id="display" />
<input type="text" id="answer" placeholder="answer" disabled/>
<button onclick="clearDisplay()">Clr</button>
<button onclick="calculateResult()">=</button>
```

## JavaScript

### `clearDisplay()`
Clears both the input and answer fields.

```js
function clearDisplay() {
  display.value = "";
  answer.value = "";
}
```

### `calculateResult()`
Evaluates the expression entered in the input field and displays the result.

```js
function calculateResult() {
  answer.value = eval(display.value);
}
```

## Usage
1. Enter a mathematical expression in the input field. eg: 2-2/2
2. Click the `=` button to evaluate the expression.
3. Click the `Clr` button to clear the fields and start over.

## Notes
- The project uses the `eval()` function, which should be used with caution to avoid security risks.

