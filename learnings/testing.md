# Testing portfolio

## 1. Check that passing a given input into our tests returns the expected output

![templatetestingjs_screenshot](https://user-images.githubusercontent.com/52511353/205373746-4c2f5f12-fa2a-4aae-a880-9b998b99ab72.png)

We used the template test-helpers.js file (above) to help us incorporate our existing code (below) into a testing framework. As you can see the TDD template file is referenced when comparing actual and expected in this test, which checks if a user can mark a task as complete.

![testingscreenshot](https://user-images.githubusercontent.com/52511353/205373236-7eb4974c-6f3e-40d6-9945-25355a914377.png)

The actual and expected results can be viewed in the console log in the screenshot below:

![testingscreenshot(3)](https://user-images.githubusercontent.com/52511353/205453159-fad5d453-6335-458f-9601-fc1cef7a2944.png)

## 2. Write tests to mimic the behaviour of a user performing different actions

This test was designed to check if the user can add a new task to their to-do list, by mimicking the process:

![testingscreenshot(2)](https://user-images.githubusercontent.com/52511353/205374991-b0340a08-a427-4abf-bd99-73b1b4ecbdea.png)

## 3. Write testable, modular functions

Rather than wrapping all code in one function, we used separate callback functions to handle each element of the functionality of our to-do list:

```js
     const getTasksFromLocalStorage = (task) => {
     ...
     }

     const addTaskItem = () => {
     ...
     }

     const deleteTask = (e) => {
     ...
     }

     const markTaskAsComplete = () => {
     ...
     }
```

## 4. Write functions that add, remove or modify DOM nodes

Our main script.js file included a deleteTask function that removes a task node from the DOM:

![screenshot(1)](https://user-images.githubusercontent.com/52511353/205384632-8a608478-affd-4c7e-80e6-94cd40e12c13.png)

## 5. Apply event listeners to HTML form elements

```html
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

The submit button in the form above in HTML triggers an onclick callback function (below). An alternative was that we could have used a `submit` event for the form instead.

![screenshot(2)](https://user-images.githubusercontent.com/52511353/205378096-f5d64707-3eff-4a0d-86c6-65b982519db0.png)

## 6. Use scope to control what variables are accessible inside functions and blocks

We delineated a number of global variables, so that they could be accessed by different functions. This included our local storage array:

```js
const input = document.querySelector("input"); // Grabs input

const list = document.querySelector(".list"); // Graps list

const submitBtn = document.getElementById("submit-btn"); // Grabs submit button

let userTasks = JSON.parse(localStorage.getItem("userTasks")) || []; // Global variable array to store user's tasks
```

Meanwhile, other varables were made specific to functions, so local in scope, by being declared inside the functions. This example declares local variables while marking a task as complete (signalled visually by ticking the box to the left of the task item and having a line run though the task), as well as updating the tasks array in Local Storage. 

![screenshot(3)](https://user-images.githubusercontent.com/52511353/205385020-0e551d10-43e4-4eb8-843e-7a0401998d47.png)

## 7. Use CSS grid to create complex layouts

We did not use CSS grid for this project, as it was not required.

## 8. Use CSS grid to make layouts that adapt to the viewport size

As mentioned in #7 above, we didn't use CSS grid for this project. However, we did make the project adapt to differing viewport sizes, as you can see with this screenshot. Our CSS utilised media queries, including flex-grow commands. 

![screenshot(4)](https://user-images.githubusercontent.com/52511353/205386328-8d4a1748-9f42-41a0-96d1-0a2327d2a6d0.png)
