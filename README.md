# DiveBridge_Week1_Task4
# 🔢 Calculator App

A modern calculator built using **HTML**, **CSS**, and **JavaScript**. This project demonstrates core JavaScript logic handling and dynamic UI updates in a responsive layout.

---

## 💻 Features

* Supports basic operations: addition, subtraction, multiplication, division
* Clear (C) and Delete (⌫) buttons
* Decimal support
* Evaluates expressions using JavaScript's `eval()`

---

## 📁 File Structure

```
project-folder/
│
├── index.html               # Main HTML structure
├── assets/
│   ├── styles/style.css     # Calculator styles
│   └── scripts/script.js    # JS logic
```

---

## 🔧 Technologies Used

* **HTML5**: Page layout and structure
* **CSS3**: Dark UI theme and responsive layout
* **JavaScript (Vanilla)**: Logic handling including input appending, evaluation, clear, and delete

---

## 🧠 JavaScript Functionalities

JavaScript file (`script.js`) handles:

* `append(value)`: Adds input to the display
* `clearDisplay()`: Clears display text
* `del()`: Deletes last character
* `calculate()`: Evaluates the expression using `eval()`

```js
function append(value) {
  document.getElementById('display').value += value;
}

function clearDisplay() {
  document.getElementById('display').value = "";
}

function del() {
  let current = document.getElementById('display').value;
  document.getElementById('display').value = current.slice(0, -1);
}

function calculate() {
  try {
    document.getElementById('display').value = eval(document.getElementById('display').value);
  } catch {
    document.getElementById('display').value = "Error";
  }
}
```

---

## 👨‍💻 Developed By

**Ahmad Rayyan**
HTML & CSS Developer
Week 1 Task for DiveBridge
