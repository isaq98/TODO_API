# Todo List API
This project is a simple Node.js/Express Todo List in order to become more familiar with the technologies we'll be using over the semester on our webapp.   


## Development Setup
You'll first need [Node.js](https://nodejs.org/) installed.

### Installing the Required Dependencies
Similar to previous instructions, please install the necessary dependencies for this API.

To install the dependencies do
```bash
cd todolist_api
npm install
```

### Starting the server
The command I use to start the server is:

You can start up the app with
```bash
npm run start:dev
```
This will cause the app to begin listening on `localhost:8000`.

#### Utilizing Postman
[Postman](https://www.postman.com/) is a platform for API development. It made testing my development significantly easier and I'd recommend it, too.

You can use the following commands to interact with the API.

**Seeing all Todo Lists**
`GET localhost:8000/api/todos`

**Creating a new Todo List**
`POST localhost:8000/api/todos`
> **Example:**
>```bash
>POST localhost:8000/api/todos
>[{title: "Todo List #4"}]

**Creating a Todo Item**
`POST localhost:8000/api/todos/[the id of the list you want to add to]/items`
> **Example:**
>```bash
>POST localhost:8000/api/todos/1/items
>{content: "Do laundry"}

**Updating a Todo List**
`PUT localhost:8000/api/todos/[the id of the list you want to add to]`
> **Example:**
>```bash
>PUT /api/todos/[the id of the list you want to add to]
>{title: "Todo List #4 - Now Updated"}

**Deleting a Todo List**
>```bash
>`DELETE localhost:8000/api/todos/[the id of the list you want to add to]/

This will then provide you a notification saying the list was deleted successfully.
