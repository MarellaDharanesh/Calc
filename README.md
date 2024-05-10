# Ex.08 Design of a Standard Calculator
## Date:

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```


index.html


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Calculator</title>
<link rel="stylesheet" href="stylee.css">
</head>
<body>
    
<div class="calculator">
    <h1> Calculator</h1>
    <h2></h2>
  <input type="text" id="display" disabled>
  <div class="buttons">
    <button onclick="appendToDisplay('1')">1</button>
    <button onclick="appendToDisplay('2')">2</button>
    <button onclick="appendToDisplay('3')">3</button>
    <button onclick="appendToDisplay('+')">+</button>
    <button onclick="appendToDisplay('4')">4</button>
    <button onclick="appendToDisplay('5')">5</button>
    <button onclick="appendToDisplay('6')">6</button>
    <button onclick="appendToDisplay('-')">-</button>
    <button onclick="appendToDisplay('7')">7</button>
    <button onclick="appendToDisplay('8')">8</button>
    <button onclick="appendToDisplay('9')">9</button>
    <button onclick="appendToDisplay('*')">*</button>
    <button onclick="appendToDisplay('0')">0</button>
    <button onclick="appendToDisplay('%')">%</button>
    <button onclick="appendToDisplay('^')">^</button>
    <button onclick="appendToDisplay('sin')">sin</button>
    <button onclick="appendToDisplay('log')">log</button>
    <button onclick="calculate()">=</button>
    <button onclick="appendToDisplay('/')">/</button>
    <button onclick="clearDisplay()">C</button>
  </div>
</div>
<script src="script.js"></script>
</body>
</html>
```

```
stylee.css

body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #93baec;
  }
  h1{
      align-items: center;
      font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
      color: rgb(27, 25, 28);
  }
  
  .calculator {
    background-color: #e2f048;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(21, 14, 14, 0.1);
  }
  h2{
      align-items: center;
      color: rgb(18, 19, 19);
  }
  
  #display {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    font-size: 24px;
    text-align: right;
    color: rgb(15, 15, 14);
  }
  
  .buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
  }
  
  button {
    padding: 15px;
    font-size: 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  button:hover {
    background-color: #080606;
  }

  script.js

  let display = document.getElementById('display');

function appendToDisplay(value) {
  display.value += value;
}

function clearDisplay() {
  display.value = '';
}

function calculate() {
  try {
    display.value = eval(display.value);
  } catch (error) {
    display.value = 'Error';
  }
}
```

## OUTPUT:
![Screenshot (143)](https://github.com/MarellaDharanesh/Calc/assets/118707669/42c8e757-af72-431a-bad6-52bedaa5728e)

![Screenshot (144)](https://github.com/MarellaDharanesh/Calc/assets/118707669/4fee6596-eda3-4fd3-b6db-60e11eb1b898)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
