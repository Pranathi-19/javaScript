# JavaScript Addition Program

## Project Description

This project demonstrates a simple **JavaScript program that adds two numbers entered by the user**.
The program also performs **input validation** to ensure that the user enters only numeric values.

If a user enters invalid input (non-numeric values), an error message will be displayed.

---

## Technologies Used

* HTML
* JavaScript
* DOM Manipulation

---

## How the Program Works

1. The user enters two values in the input fields.
2. When the **Add** button is clicked, the `validation()` function is called.
3. The function checks whether the inputs are valid numbers using `isNaN()`.
4. If invalid input is detected, an error message is displayed.
5. If both inputs are valid numbers, the `addition()` function calculates the sum.
6. The result is displayed dynamically on the webpage.

---

## Project Structure

```
javaScript
│
├── addition.html
├── README.md
└── images
    ├── addition_result.png
    ├── invalid_input_num1.png
    └── invalid_input_num2.png
```

---

## Code Overview

### Validation Function

This function checks whether the user input values are numbers.

```javascript
function validation(){
    let number1=parseInt(document.getElementById("number1").value);
    let number2=parseInt(document.getElementById("number2").value);

    if(isNaN(number1) || isNaN(number2)){
        document.getElementById("result_id").innerHTML="Please Enter numbers only";
    }
    else{
        addition();
    }
}
```

### Addition Function

This function calculates the sum of the two numbers and displays the result.

```javascript
function addition(){
    let number1=parseInt(document.getElementById("number1").value);
    let number2=parseInt(document.getElementById("number2").value);
    let sum = number1 + number2;

    document.getElementById("result_id").innerHTML="The Sum is = " + sum;
}
```

---

## Program Output

### Addition Result

![Addition Result](images/addition_result.png)

### Invalid Input for First Number

![Invalid Input Number1](images/invalid_input_num1.png)

### Invalid Input for Second Number

![Invalid Input Number2](images/invalid_input_num2.png)

---

## Features

* Simple user interface
* Input validation for numeric values
* Dynamic result display using JavaScript
* Error handling for invalid input

---

## Author

**Pranathi Guddenka**
