# Todo List Restful API

## Overview
The Todo List Restful API provides a simple interface for managing a list of todo items. Users can create, read, update, and delete todo entries.

## Features
- Retrieve all todo lists
- Create a new todo list
- Update an existing todo list
- Delete a todo list

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/todo-list-api.git
2. Navigate to the project directory:
   `cd todo-list-api`
3. Install extensio OpenAPI in Vscode
4. Open With OpenAPI
   
# Usage

The API is documented using OpenAPI 3.0.3 specification. Below is a summary of the available endpoints.

## Get All Todo Lists
- **Endpoint**: `/todoList`
- **Method**: `GET`
- **Description**: Retrieve all active todo lists.
- **Parameters**:
  - `include done` (query, optional, boolean): Include completed todo lists (default: false).
  - `name` (query, optional, string): Filter todo lists by name.
- **Responses**:
  - **200**: Successful retrieval of todo lists.

## Create New Todo List
- **Endpoint**: `/todoList`
- **Method**: `POST`
- **Description**: Create a new todo list entry.
- **Request Body**:
  - **Required**: true
  - **Content**: JSON object containing name, priority, and tags.
- **Responses**:
  - **200**: Successful creation of a todo list.

## Update Existing Todo List
- **Endpoint**: `/todoList/{todoListId}`
- **Method**: `PUT`
- **Description**: Update an existing todo list entry.
- **Parameters**:
  - `todoListId` (path, required, string): ID of the todo list to update.
- **Request Body**:
  - **Required**: true
  - **Content**: JSON object containing name, priority, and tags.
- **Responses**:
  - **200**: Successful update of a todo list.

## Delete Existing Todo List
- **Endpoint**: `/todoList/{todoListId}`
- **Method**: `DELETE`
- **Description**: Delete an existing todo list entry.
- **Parameters**:
  - `todoListId` (path, required, string): ID of the todo list to delete.
- **Responses**:
  - **200**: Successful deletion of a todo list.
  - **404**: Todo list not found.

# Security
The API uses an API key for authentication. Include the API key in the header of each request with the name X-API-Key.

# License
This project is licensed under the APACHE 2.0 License - see the LICENSE file for details.

# Contact
- **Author**: Defrizal Yahdiyan Risyad
- **Email**: defrijay@upi.edu
- **URL**: Kemakom


