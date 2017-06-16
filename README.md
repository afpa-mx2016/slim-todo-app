# simple single-user Slim todo app

example definition of REST webservice to create/read/update/delete/ tasks


 - it uses [Slim](https://www.slimframework.com/) as php Framework




## install

Create a database, and import initial SQL definition file `resources/todo-app.sql`.
Tune your settings `src/settings.php`

Download dependencies ( need [composer](https://getcomposer.org/) )

```shell
composer install
```

## run

`composer start`


## available API

 - get all todos:

 ```
 curl http://localhost:8080/api/v1/todos
 ```

 - get todo with id=6:

 ```
 curl http://localhost:8080/api/v1/todos/6
 ```

 - update todo with id=6:

 ```
 curl -XPUT -d '{"task":"my task", "priority":1}' http://localhost:8080/api/v1/todos/6
 ```

 - delete todo with id=6:

 ```
 curl -XDELETE  http://localhost:8080/api/v1/todos/6
 ```

 - create todo:

 ```
 curl -XPOST -d '{"task":"my task", "priority":1}' http://localhost:8080/api/v1/todos
 ```


Sample mini-js app available at `http://localhost:8080/todos_object.html`
