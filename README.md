# Vanilla REST API Inspired by Eli Berdensky

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

This educational project is a simple Vanilla REST API inspired and adapted from the teachings of Eli Berdensky. The goal is to provide a hands-on learning experience for building a basic RESTful API using Golang.

## Features

- RESTful endpoints for basic CRUD operations.
- In-memory storage for simplicity and ease of understanding.
- Go modules for managing dependencies.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Go installed on your machine.
- Basic understanding of Golang.

## Getting Started

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/vanilla-rest-api.git
   cd vanilla-rest-api


2. Run the Application:

   ```bash
   go run main.go

## License
This project is licensed under the MIT License.

## API Endpoints

- `POST /task/`: Create a task and return its ID.
- `GET /task/{taskid}`: Retrieve a single task by ID.
- `GET /task/`: Retrieve all tasks.
- `DELETE /task/{taskid}`: Delete a task by ID.
- `GET /tag/{tagname}`: Retrieve a list of tasks with the specified tag.
- `GET /due/{yy}/{mm}/{dd}`: Retrieve a list of tasks due by the specified date.

### Creating a New Task (POST /task/)

To create a new task, send a `POST` request to `http://localhost:8080/task/` with the following JSON payload:

    ```json
    {
    "text": "Sample Task",
    "tags": ["tag1", "tag2"],
    "due": "2022-02-21T12:00:00Z"
    }

