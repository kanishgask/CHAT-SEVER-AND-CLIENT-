# CHAT-SEVER-AND-CLIENT-
# 🗨️ Java Chat Application using TCP Sockets

## 📌 Project Description

This is a simple **Java-based chat application** that demonstrates a basic client-server communication model using **TCP sockets**. Both the client and server can send and receive messages until either party sends `"stop"` to terminate the connection.

---

## 🎯 Objective

To develop a Java application that allows two-way communication (chat) between a client and a server using TCP sockets.

---

## 📂 Project Files

- `ChatServer.java`: The server-side socket program.
- `ChatClient.java`: The client-side socket program.
- `README.md`: Documentation and execution instructions.

---

## 🔄 Algorithm

### Server
1. Import necessary packages.
2. Create a `ServerSocket` on port `6666`.
3. Accept a connection using `accept()`.
4. Set up input and output streams to communicate.
5. Use `readUTF()` to receive and `writeUTF()` to send messages.
6. Continue communication until the message `"stop"` is received.
7. Close all resources.

### Client
1. Import necessary packages.
2. Create a `Socket` to connect to the server on `localhost:6666`.
3. Set up input and output streams.
4. Send messages to the server using `writeUTF()`.
5. Receive server messages using `readUTF()`.
6. Continue communication until the message `"stop"` is sent.
7. Close all resources.

---

## 🔧 How to Compile and Run

### 🛠️ Prerequisites
- JDK installed (e.g., JDK 1.7+)
- Java environment variables properly set

### 💻 Compilation Steps

1. Open two command prompts — one for the server, one for the client.
2. Compile the server:
    ```bash
    javac ChatServer.java
    ```
3. Compile the client:
    ```bash
    javac ChatClient.java
    ```

### ▶️ Execution Steps

1. Run the server in the first terminal:
    ```bash
    java ChatServer
    ```
2. Run the client in the second terminal:
    ```bash
    java ChatClient
    ```

---

## 🖥️ Sample Interaction

**OUTPUT**
TO SERVER : Hi Server!
SERVER SAYS : Hello Client, welcome!
TO SERVER : How are you?
SERVER SAYS : I’m doing well, thank you!
TO SERVER : stop
SERVER SAYS : Bye!

CLIENT SAYS : Hi Server!
TO CLIENT : Hello Client, welcome!
CLIENT SAYS : How are you?
TO CLIENT : I’m doing well, thank you!
CLIENT SAYS : stop
TO CLIENT : Bye!
**OUTPUT CLIENT**
TO SERVER : Hi Server!
SERVER SAYS : Hello Client, welcome!
TO SERVER : How are you?
SERVER SAYS : I’m doing well, thank you!
TO SERVER : stop
SERVER SAYS : Bye!
