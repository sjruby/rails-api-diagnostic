# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To persist data and interact with server requests as designed by the devolper
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
// your response here
```

Which layer in the MVC pattern communicates with the model?

```md
The controller tells the model what to do
```

Why don't we use views in our interpretation of the MVC pattern?

```md
I don't know what this asking, we do use use views in the MVC pattern, its the V.
```

What does C.R.U.D stand for?

```md
CREATE READ UPDATE DESTROY
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
In the controler
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index show create update delete
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. Server sends the URL to router
2. Router looks at the GET request and URL trys to find a controller for people to determin what the GET is for
3. The controller takes the ID from the URL(#1) and sends taht over to model to ask it to create a view of the person with ID #1 by rendering some JSON based on the parameters
4. the controler passes the rendered JSON back to the router/server
5. the router/server pass the rendered JSON back to the client which does what it wsa programed to with that JSON.
```

What is the command to generate a new rails-api app?

```bash
rails new API
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
db:drop
db:create
db:migrate
db:seed
db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold Pets name:string age:integer
```
