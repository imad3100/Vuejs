# VUE JS TodoList ADD,Delete,Update 


# Code Explications 

The HTML Consists of 3 Parts : a form to add a new todo , a todo-nav to switch between all,active,completed todos ,
a todo-list which represents todo item.

a switch between all,active,completed done by modifying boolean variables :all:true , active:false, completed:false .
 
the input variable is binded with form input using v-model  .

when a click on button add() is called to push input to tasks array.

a task is not editable by defautlt , it becomes editable when click on edit button , then it's replaced by a form ,
and the new edit form is binded with task.text using v-model to make changes.

delet() function takes index of tasks and removes it using splice().


actives, completeds tasks properties are computed by doing a filter on tasks array based on task.done condition . 
