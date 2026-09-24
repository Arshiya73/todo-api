# Todo REST API

This is a simple Todo REST API that I built using Node.js, Express.js, and MongoDB as part of my backend assignment.

The API allows users to create, view, update, and delete todo items. Todo data is stored in MongoDB.

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose

## Features

- Create a new todo
- Get all todos
- Get a todo using its ID
- Update an existing todo
- Delete a todo
- Validate todo titles
- Handle invalid IDs and missing todos
- Store todo data in MongoDB

## Getting Started

### 1. Install dependencies

bash
npm install


### 2. Configure environment variables

Create a .env file in the project root and add your MongoDB connection string:

env
PORT=5000
MONGO_URI=your_mongodb_connection_string


Replace the placeholder with your MongoDB connection string.

### 3. Run the server

bash
npm start


The server will run on port 5000, unless another port is configured.

## API Routes

| Method | Route | Description |
|---|---|---|
| POST | /todos | Create a todo |
| GET | /todos | Get all todos |
| GET | /todos/:id | Get a todo by ID |
| PUT | /todos/:id | Update a todo |
| DELETE | /todos/:id | Delete a todo |

## Example

To create a todo, send a POST request to /todos with a JSON body:

json
{
  "title": "Buy groceries",
  "description": "Milk, eggs, bread"
}


## Error Responses

The API returns JSON error messages for invalid input and missing todos, along with suitable HTTP status codes.

## Environment File

A .env.example file is included to show the required environment variables. The actual .env file should not be committed to the repository.
## LIVE API URL
https://todo-api-4kcw.onrender.com 
