#Stsif_chatApp

##An online chat application implemented in Java. It includes a server and client application that allow to communicate within sockets. Through The server the users connect and broadcasts messages to all connected users.


## Implementation

### Server

The `ChatServer' class implements the server-side logic. It Listens for incoming incoming connections from client,
 assigns user IDs, and broadcasts Thier messages to all connected clients. The server enables users to chat and messages can be sent from the server console to all clients.

#### Key Components:
- `ServerSocket`: Listens for incoming connections on a specified port.
- `ClientHandler`: Handles individual client connections and processes their messages.
- `handleServerInput()`: Reads input from the server console and broadcasts it to all clients.
- `broadcast(String message)`: Sends a message to all connected clients.

### Client

`ChatClient` class implements the client-side logic. It connects to the server, sends messages to it, and displays messages received from the server.

#### Key Components:
- `Socket`: Connects to the server.
- `PrintWriter`: Sends messages to the server.
- `BufferedReader`: Receives messages from the server.
- `Thread`: Handles incoming messages from the server in a separate thread.

##Runing

### Prerequisites

- Java Development Kit (JDK) 8 or higher.

### How to Run the Application

1. Compile the Code:
   First, Open a terminal or command prompt, navigate to the directory containing the `.java` files, and compile the code using:
   ```sh
   javac ChatServer.java ChatClient.java

2. Run the Server: next run Server 
'java ChatServer'

3. Run the Client class: vis  another terminal or command prompt 'java ChatClient'


### How to Usage
1.Run the server.
2. Run the Client class.
3. Start chatting 






