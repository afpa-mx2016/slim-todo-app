##simple single-user Slim todo app

use of REST webservice to create/read/update/delete/ tasks

enabled *CORS* header to make it available within your network.

#install

Prepare your database, see `resources/todo-app.sql` and tune your `src/settings.php`

Download dependencies ( need `composer` )

```shell
composer install
```

#run

`composer start`


##available API 

 - get all todos:

 `GET http://localhost:8080/api/v1/todos`

 - get todo with id=6:

 `GET http://localhost:8080/api/v1/todos/6`

 - update todo with id=6:

 `PUT http://localhost:8080/api/v1/todo/6`

 - delete todo with id=6:

 `DELETE http://localhost:8080/api/v1/todo/6`

 - create todo:

 `POST http://localhost:8080/api/v1/todo` 


Sample mini-js app available at `http://localhost:8080/todos_object.html`


