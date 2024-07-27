# Simple HTTP Server in C

This project is a basic implementation of an HTTP server written in C. The server listens on port 8080 and responds with a simple HTML page to any HTTP GET request.

## Features

- Handles incoming HTTP GET requests.
- Sends a basic HTML response with a "Hello, World!" message.

## Getting Started

### Prerequisites

- A C compiler (e.g., `gcc`).
- POSIX-compliant operating system (e.g., Linux, macOS).

### Compilation and Execution

1. **Clone the repository**:
    ```sh
    git clone https://github.com/keremishik/http-server.git
    cd http-server
    ```

2. **Compile the server**:
    ```sh
    gcc -o server server.c
    ```

3. **Run the server**:
    ```sh
    ./server
    ```

4. **Access the server**:
   Open your web browser and navigate to `http://localhost:8080`.

## Code Overview

The main parts of the server code include:

- **Socket creation**: Sets up a socket to listen for incoming connections.
- **Binding**: Binds the socket to a specific port (8080).
- **Listening**: Listens for incoming connection requests.
- **Accepting connections**: Accepts and handles incoming connections.
- **Sending responses**: Sends a basic HTML response back to the client.

### Example HTML Response

The server responds with the following HTML:

```html
HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 49

<html><body><h1>Hello, World!</h1></body></html>
