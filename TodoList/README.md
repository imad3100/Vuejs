# VUE JS TodoList ADD,Delete,Update 


# Code Explications 

The HTML Consists of 3 Parts : a form to add a new todo , a todo-nav to switch between all,active,completed todos ,
a todo-list which represents todo item.

a switch between all,active,completed done by modifying boolean variables :all:true , active:false, completed:false .
 
the input variable is binded with form input using v-model  .

when a click on button add() is called to push input to tasks array.

a task is not editable by defautlt , it becomes editable when click on edit button , then it's replaced by a form ,
and task.text is stored on edits array according to his index , this is done to set task.text to a default value
of the edit form input using v-model between the edit input and edits[index].

delet() function takes index of tasks and removes it using splice().

edite() takes index of task ,replaces task.text with it's new value in edits array.

actives, completeds tasks properties are computed by doing a filter on tasks array based on task.done condition . 
