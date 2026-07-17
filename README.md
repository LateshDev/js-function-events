# js-function-events
 JavaScript Functions & Events
---

📚 What You’ll Learn

- Functions & their types
- Parameters vs Arguments
- Return values
- Pure & Impure logic
- Arrow functions
- Events & event handling

---

🔧 Functions in JavaScript

📌 What is a Function?

A function is a reusable block of code designed to perform a specific job.
```
function greet() {
  console.log("Hello");
}

greet();

```
---

🎯 Why Functions Matter

- 🔁 Avoid repeating code
- ♻️ Reusable logic
- 🧹 Cleaner & organized code
- 🐞 Easier debugging
- 👀 Improves readability

---

✅ Best Practices

- Keep functions short & focused
- One function = one responsibility
- Use clear and meaningful names
- Break big logic into smaller parts

---

🧠 Parameters vs Arguments

```
function add(a, b) {
  return a + b;
}

add(2, 3);

```
- Parameters → variables in function ("a", "b")
- Arguments → actual values ("2", "3")

---

🔙 Return Statement

```
function square(num) {
  return num * num;
}

```
- Sends result back
- Stops execution immediately

⚠️ Code after "return" will not run

---

🔄 Function vs Procedure

Type| Behavior
Function| Takes input + returns output
Procedure| Performs action only

👉 In JavaScript, both are treated as functions

---

⚖️ Pure vs Impure Functions

🟢 Pure Function

- Same input → same output
- No external changes

```
function add(a, b) {
  return a + b;
}
```
---

🔴 Impure Function

- Depends on outside data
- Can modify variables
```
let count = 0;

function increment() {
  count++;
}
```
---

🛠️ Ways to Define Functions

1. Function Declaration

```
function greet(name) {
  return "Hi " + name;
}
```
---

2. Function Expression

```
const greet = function(name) {
  return "Hi " + name;
};
```
---

3. Arrow Function

```
const greet = (name) => {
  return "Hi " + name;
};
```
---

⚡ Arrow Function Shortcuts

```
const add = (a, b) => a + b;   // implicit return
const square = n => n * n;     // single parameter
```
---

🎯 JavaScript Events

📌 What is an Event?

An event is any interaction done by the user on a webpage.

👉 Examples:

- Click
- Typing
- Scrolling
- Form submission

---

🎧 Listening to Events

```
button.addEventListener("click", () => {
  console.log("Clicked!");
});
```
---

🔁 Callback Function

button.addEventListener("click", changeColor);

❌ Avoid:
```
changeColor();
```

👉 Because it runs immediately instead of waiting

---

📦 Event Object

```
button.addEventListener("click", (event) => {
  console.log(event.target);
  console.log(event.type);
});
```
Useful properties:

- "event.target" → element clicked
- "event.type" → event name

---

📊 Common Events

```
Event| Meaning
click| Mouse click
dblclick| Double click
keydown| Key pressed
keyup| Key released
input| Typing input
submit| Form submitted
scroll| Page scroll
load| Page loaded

```
---

🧩 Event Handling Steps

```
// Step 1: Select element
const btn = document.querySelector(".btn");

// Step 2: Create function
function changeColor() {
  document.body.style.background = "lightblue";
}

// Step 3: Attach event
btn.addEventListener("click", changeColor);
```

👉 Flow: Select → Listen → Perform

---

❌ Removing Events

```
btn.addEventListener("click", changeColor);
btn.removeEventListener("click", changeColor);

```
Why remove?

- One-time actions
- Save memory
- Disable features

---

🛡️ Graceful Degradation

Your website should still work even if JavaScript is disabled.

Best Approach:

- Build strong HTML structure first
- Use JS only for enhancement
- Don’t rely fully on JavaScript

---

⚡ Quick Recap

- Functions = reusable logic blocks
- Parameters ≠ Arguments
- "return" sends values back
- Pure functions are predictable
- Arrow functions are shorter syntax
- Events bring interactivity
- Use "addEventListener()" to handle events
- Follow pattern: Select → Listen → Perform

---

✍️ Author

Latesh Padaliya
