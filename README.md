# JavaScript Basics

## When to Use `let` and `const` to Create Variables

- Use `let` for variables that **you want to change**.
- Use `const` for variables that **should not change**.

---

## How to Link JavaScript to Your HTML File

### 1. External Method
Create a JavaScript file (e.g., `script.js`) and link it in your HTML `<head>` or at the end of the `<body>` section using the following code:

```html
<script src="script.js"></script>
```

### 2. Internal Method
You can also write JavaScript code directly inside your HTML file:

```html
<script>
  console.log("Hi, I am JS");
</script>
```

---

## JavaScript Functions (Summary)

Here are some basic function examples:

```js
function greet() {
  console.log("Hello World");
}

greet();

function calculateSum(x, y) {
  console.log(x + y);
}

calculateSum(5, 10);
```

---

## How to Change the Content of Your HTML with JavaScript

To change the content of an HTML page using JavaScript:

1. Assign an `id` to the HTML element.
2. Call the function using an `onClick` attribute in a button or any other HTML element.

Example:

```html
<p id="change-me">Good Morning All</p>
<button onClick="handleChange()">Click Me</button>
```

In your JavaScript file:

```js
function handleChange() {
  document.getElementById("change-me").innerHTML = "Good Evening All";
  document.getElementById("change-me").style.color = "green";
}
```

---

## JavaScript Arrays (Summary)

Arrays are used to store multiple values in a single variable. They are declared using square brackets `[]`.

Example:

```js
const myArray = [1, 2, 3, 4, 5];
const anotherArray = ["a", "b", "c"];
const mixedArray = [1, "a", 2, "b", 3, "c"];
const carCollection = ["Toyota", "BMW", "Honda"];
```

### Accessing Elements

To get an element from an array, use its index (starting from 0):

```js
console.log(myArray[0]); // 1
console.log(carCollection[2]); // Honda
```

### Adding Items

To add an item to an array, use the `push` method:

```js
carCollection.push("Mercedes");
carCollection.push("Kia");
console.log(carCollection);
```

### Removing Items

To remove the last item from an array, use the `pop` method:

```js
carCollection.pop();
console.log(carCollection);
```

### Checking Array Length

To check the number of elements in an array, use the `length` property:

```js
console.log(carCollection.length);
```

---

## JavaScript Objects (Summary)

Objects store data in key-value pairs and are declared using curly braces `{}`.

Example:

```js
const aboutMe = {
  myName: "Damian",
  age: 2,
  title: "Developer",
};
```

### Accessing Object Properties

You can access object properties using dot notation:

```js
console.log(aboutMe.myName); // Damian
console.log(aboutMe.title); // Developer
```

### Adding Data to Objects

To add new properties to an object:

```js
aboutMe.location = "New York";
console.log(aboutMe);
```


