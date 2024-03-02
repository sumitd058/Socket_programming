# Socket_programming
Chat Application README

This README provides an overview of the chat application implemented using socket programming in C.

1. Overview:
The chat application follows a client-server model where clients connect to a central server to exchange messages with each other. The server listens for incoming connections on a specified port and handles each client connection in a separate thread. Messages sent by any client are broadcasted to all other connected clients.

2. Server Setup:
   - To run the server, compile and execute the server.c file.
   - The server listens for client connections on a specified port (default port is usually 8000, but it can be changed as needed).
   - Once the server is running, it waits for clients to connect.

3. Client Connection:
   - Clients need to connect to the server using its IP address and port number.
   - To run a client, compile and execute the client.c file.
   - Clients should provide the server's IP address and port number to establish a connection.
   - Once connected, clients can send and receive messages with other connected clients.

4. Message Broadcasting:
   - Messages sent by any client are broadcasted to all other connected clients.
   - This ensures that messages sent by one client are visible to all participants in the chat.

5. Thread Management:
   - Threading is used to manage multiple client connections concurrently without blocking.
   - Each client connection is handled in a separate thread, allowing the server to handle multiple clients simultaneously.

6. Message Protocol:
   - A simple protocol is defined for communication between clients and the server.
   - The protocol includes message types (e.g., chat messages, system messages), sender information, timestamps, etc.

7. Running the Application:
   - Clone the repository or download the source files.
   - Compile the server.c and client.c files using a C compiler (e.g., gcc).
   - Run the compiled server executable to start the server.
   - Run the compiled client executables to connect to the server and start chatting.

8. Additional Notes:
   - Ensure that the necessary dependencies are installed for socket programming in C.
   - Customize the port number, message protocol, and other settings as per requirements.
   - Implement error handling and security measures as needed, especially in a production environment.

9. Authors:
   -Sumit Dubey
   
11. Contact:
    - sumitd058@gmail.com

Please refer to the specific documentation or source code for detailed instructions and implementation details. 
