# Python Networking Lab

This project demonstrates basic **client-server communication** using Python's `socket` library. The **server** listens for connections, while the **client** connects to the server, sends a message, and receives a response.

---

### Behavior Overview

1. **Server (`server.py`):**
   - Starts and listens on `127.0.0.1:12345`.
   - Accepts a connection from the client.
   - Receives a message from the client.
   - Echoes the message back to the client.

2. **Client (`client.py`):**
   - Connects to the server at `127.0.0.1:12345`.
   - Sends a message: `"Hello server, this is from the client"`.
   - Receives the same message echoed back from the server.
   - Prints the server's response.

---

### How to Run

1. Start the **server** first:
   ```bash
   python server.py
   ```
   - The server will wait for a connection from the client.

2. Start the **client** in a separate terminal:
   ```bash
   python client.py
   ```
   - The client connects to the server, exchanges messages, and exits.

---

### Expected Output

- **Server Terminal:**
  ```
  Server listening on 127.0.0.1:12345...
  Connection established with ('127.0.0.1', <port>)
  Received: Hello server, this is from the client
  ```

- **Client Terminal:**
  ```
  Received from server: Hello server, this is from the client
  ```