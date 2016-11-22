#simple single-user Slim todo app

use of REST webservice to create/read/update/delete/ tasks

enabled *CORS* header to make it available within your network.

Prepare your database, see `resources/todo-app.sql` and tune your `src/settings.php`

To run the application in development, you can run this command. 
`composer start`

now browse to `http://localhost:8080/todos_object.html`

##API available
GET http://localhost:8080/api/v1/todos
PUT http://localhost:8080/api/v1/todo/6 
DELETE http://localhost:8080/api/v1/todo/6 
POST http://localhost:8080/api/v1/todo 





