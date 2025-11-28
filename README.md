# Interactive Task Manager

## Project Description
This project aims to create a task manager web application using HTML, CSS, and JavaScript. Development should focus on functionality, user experience, and clean code implementation to help users organize and track their tasks efficiently.

## Project Requirements
This project requires the application to allow users to create, modify, and delete tasks dynamically. There must be a dedicated section of the webpage to display each task using JavaScript, and each task should be styled to indicate priority, importance, and completion status. The application is also required to log task updates to the browser console using JSON.stringify(). Finally, the project must be visually appealing, user-friendly, and well-documented.

## Specific Requirements

### User Interface
- An input field for users to enter a task name.
- A dropdown menu where users can select task priority.
- A checkbox for marking tasks as important.
- A checkbox for marking tasks as complete.
- A submit button for adding tasks to the list.
- A delete button for removing tasks from the list.
- A date to show when the task was added.
- An HTML **\<div>** element with the id "taskmanager" for tasks to be displayed dynamically.
- Completed tasks must have a strikethrough using the JavaScript **.style** property.
- Important tasks must be highlighted red using the JavaScript **.style** property.

### JavaScript Requirements
- **Event Handling & DOM Manipulation**
    - Users should be able to submit tasks via the form.
    - Tasks must be displayed dynamically in the **#taskmanager** div using **.innerHTML**.
    - Users must be able to delete tasks.
    - Users must be able to toggle task completion.
    - Each task must display the date it was created using the **Date** object.

- **Task Data Structure**
    - Tasks must be stored in an array of objects with the following properties:
    ```
    {
        id (int): taskId,
        name (str): "Task Name",
        priority (str): "Task Priority",
        isImportant (bool): importanceBool,
        isCompleted (bool): completionBool,
        date (Date): dateCreated
    }
    ```
    - Whenever a task is added, updated, or deleted, the full task list must be logged in the console using `console.log(JSON.stringify(tasks));`.

### Non-Functional Requirements
- The application must be coded using no external libraries or frameworks.
- The code must be clean with proper indentation, meaningful variable names, and comments.
- The UI should be responsive and visually intuitive.
- The form must prevent invalid input.