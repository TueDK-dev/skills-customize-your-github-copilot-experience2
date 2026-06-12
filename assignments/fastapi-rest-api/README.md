# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a REST API using the FastAPI framework to practice endpoint design, request handling, JSON responses, and error handling in Python.

## 📝 Tasks

### 🛠️ Create Basic API Endpoints

#### Description
Create the FastAPI application and define endpoints for the API root and for retrieving items by ID.

#### Requirements
Completed program should:

- Create a `FastAPI()` application instance
- Define a root endpoint at `GET /` that returns a welcome message
- Define a `GET /items/{item_id}` endpoint that returns item details as JSON
- Use a dictionary or list to store items in memory for testing
- Return a 404 error if the requested item does not exist


### 🛠️ Add Item Creation and Updates

#### Description
Implement endpoints for creating new items and updating existing items using request bodies and validation.

#### Requirements
Completed program should:

- Define a Pydantic model to validate item data
- Implement `POST /items/` to create a new item from JSON request data
- Implement `PUT /items/{item_id}` to update an existing item
- Return the created or updated item as JSON
- Use proper HTTP status codes for success and errors


### 🛠️ Support Query Parameters and Error Handling

#### Description
Add support for optional query parameters and robust error handling for API requests.

#### Requirements
Completed program should:

- Support an optional query parameter on an endpoint (for example, `?category=...` or `?limit=...`)
- Return a helpful error message when an item is missing or invalid data is sent
- Include example usage in the README such as:
  ```bash
  curl http://localhost:8000/items/1
  curl -X POST http://localhost:8000/items/ -H "Content-Type: application/json" -d '{"name":"Pencil","price":1.50}'
  ```
