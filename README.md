# Simple CRUD API with Go and Gorilla Mux

This is a simple CRUD (Create, Read, Update, Delete) API implemented in Go using the Gorilla Mux router.

## Features

- Retrieve a list of movies
- Retrieve a single movie by ID
- Create a new movie
- Update an existing movie
- Delete a movie by ID

## Prerequisites

Make sure you have Go installed on your machine. You can download and install it from [here](https://golang.org/dl/).

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Yash-sudo-web/GolangCRUD

2. Navigate to the project directory:

   ```bash
   cd GolangCRUD

3. Build and run the application:

   ```bash
   go build . && ./crud

## API Endpoints
- GET /movies: Retrieve a list of all movies.
- GET /movies/{id}: Retrieve a single movie by its ID.
- POST /movies: Create a new movie.
- PUT /movies/{id}: Update an existing movie by its ID.
- DELETE /movies/{id}: Delete a movie by its ID.

## Usage
You can use tools like cURL or Postman to interact with the API endpoints. Here are some examples:
- Get all movies:

  ```bash
  curl http://localhost:8000/movies
  
- Get a movie by ID:
  
  ```bash
  curl http://localhost:8000/movies/1

- Create a new movie:

  ```bash
  curl -X POST -H "Content-Type: application/json" -d '{"isbn":"123456","title":"New Movie","director":{"firstname":"Jane","lastname":"Doe"}}' http://localhost:8000/movies

- Update an existing movie:

  ```bash
  curl -X PUT -H "Content-Type: application/json" -d '{"isbn":"123456","title":"Updated Movie","director":{"firstname":"Jane","lastname":"Doe"}}' http://localhost:8000/movies/1

- Delete a movie by ID:

  ```bash
  curl -X DELETE http://localhost:8000/movies/1

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the [MIT License](https://github.com/Yash-sudo-web/GolangCRUD/blob/master/LICENSE).
