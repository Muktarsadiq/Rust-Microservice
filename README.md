# Microservice Project

This project is a Rust-based microservice for managing messages with a PostgreSQL database backend. It provides a RESTful API to store, retrieve, and display messages. The microservice is built using the following technologies:

- **Hyper**: HTTP server library
- **Diesel**: ORM for database interactions
- **Maud**: HTML template engine
- **Serde**: JSON serialization/deserialization
- **Env_logger**: Logging utility

## Features

- **POST `/`**: Add a new message to the database. Accepts `message` and `username` parameters in the request body.
- **GET `/`**: Retrieve and display a list of messages in an HTML format. Supports optional query parameters `before` and `after` for filtering messages by timestamp.

## Requirements

- **Rust (Nightly)**: Required for `#![feature(proc_macro_hygiene)]`
- **PostgreSQL**: Database backend
- **Environment Variables**: Configure the database connection string via the `DATABASE_URL` environment variable. Defaults to `postgresql://postgres@localhost:5432`.

## Setup and Usage

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
2. Run docker-compose up to start the service.
