# To-Do List
Celeste Robinson

## Objective

This was one of the first projects I did after learning the basics of JavaScript and jQuery. The goal was to create a program that allows the user to add tasks to a todo list. They can then cross them off when they have finished. The user can also add multiple things to the todo list if they are separated by a comma.

### Web View
![to-do list](screenshots/items-added.png)

## Technologies Used
* HTML, CSS, JavaScript, jQuery

## Code Examples
In this project, I used JavaScript and jQuery. Below is my JavaScript function that adds a new task to my list of tasks. We create a new ```li``` element, and 

```
function addTask(newTask) {
        var newLi = document.createElement("li");
        var ul = document.getElementById("list");
        var task = document.createTextNode(newTask);
        newLi.appendChild(task);
        newLi.setAttribute('id', newTask);
        ul.appendChild(newLi);
        newLi.onclick = strikethrough;
    }
```