# Testing portfolio

## 1. Check that passing a given input into our tests returns the expected output

![templatetestingjs_screenshot](https://user-images.githubusercontent.com/52511353/205373746-4c2f5f12-fa2a-4aae-a880-9b998b99ab72.png)

We used the template test-helpers.js file (above) to help us incorporate our existing code (below) into a testing framework. As you can see the TDD template file is referenced when comparing actual and expected in this test, which checks if a user can mark a task as complete.

![testingscreenshot](https://user-images.githubusercontent.com/52511353/205373236-7eb4974c-6f3e-40d6-9945-25355a914377.png)

## 2. Write tests to mimic the behaviour of a user performing different actions

This test is designed to check if the user can add a new task to their to-do list:

![testingscreenshot(2)](https://user-images.githubusercontent.com/52511353/205374991-b0340a08-a427-4abf-bd99-73b1b4ecbdea.png)

## 3. Write testable, modular functions

Rather than wrapping all code in one function, we used separate functions to handle each element of the functionality of our to-do list:

```
const getTasksFromLocalStorage()

const addTaskItem()

const deleteTask()

const markTaskAsComplete()
```

## 4. Write functions that add, remove or modify DOM nodes

Our main script.js file includes a deleteTask function that removes a task node from the DOM:

![testingscreenshot(2)](https://user-images.githubusercontent.com/52511353/205377304-4062c1b2-447e-4374-88d2-883813cb19bb.png)

## 5. Apply event listeners to HTML form elements

```
<form class="form" action="" id="to-do-input">
     <input
       class="form-input"
       required
       aria-label="Enter task"
       type="text"
       id="to-do"
       name="to-do"
       placeholder="Enter a to-do item"
        />
        <button type="submit" id="submit-btn">Submit</button>
    </form>
```

The submit button in the form above in HTML triggered an onclick callback function. 

![screenshot(2)](https://user-images.githubusercontent.com/52511353/205378096-f5d64707-3eff-4a0d-86c6-65b982519db0.png)

## 6. Use scope to control what variables are accessible inside functions and blocks

We delineated a number of global variables, so that they could be accessed by different functions. This included our local storage array:

```
// grabs input
const input = document.querySelector("input");
// grabs list
const list = document.querySelector(".list");
// grabs submit button
const submitBtn = document.getElementById("submit-btn");
// Array to store user's tasks
let userTasks = JSON.parse(localStorage.getItem("userTasks")) || [];
```

Meanwhile, other varables were made specific to functions, so local in scope, by being declared inside the functions. This example declares local variables while marking a task as complete (signalled visually by having a line though the task), as well as updating the tasks array in Local Storage. 

![screenshot(3)](https://user-images.githubusercontent.com/52511353/205381752-9fab7dd1-a477-495b-96c1-deebfc27a8b5.png)

## 7. Use CSS grid to create complex layouts

We did not use CSS grid for this project, as it was not required.

## 8. Use CSS grid to make layouts that adapt to the viewport size
