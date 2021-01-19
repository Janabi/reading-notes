# Message Queues

## Review, Research, and Discussion

### What does it mean that web sockets are bidirectional? Why is this useful?
**Bidrectional means that the sender and resiever are in connect with each other and whatever you do, it will directly shows to the other side and vice versa.**

### Does socket.io use HTTP? Why?
Definitely, it will use http to enable the socket.io to connect to the host and port.

### What happens when a client emits an event?
**The emit will send the data to the main file (server) where you can console log it.**

### What happens when a server emits an event?
**Emit the data that could be an error or a real data as an object to the client side files.**

### What happens if a client “misses” an event?
**Nothing will be sent or recieved from the client and server sides.**

### How can we mitigate this?
**By determine a certain event name that could be used as a key word to the all files including the client and server sides.**

## Document the following Vocabulary Terms

- **_Web Socket_**  is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

- **_Socket.io_** used by a real-time, bidirectional and event-based communication.

- **_Client_** the side where it will send a data by an action name.

- **_Server_** the side where it will recieve the data and emit it to the rest.

## Preparation Materials

**The material where talking about building a real chat application that could be implemented in the browser using the express and socket.io modules. Also, there will taking more about the room and namespace, and each room will have a multiple namespaces, where could make the user possibly joined any group chat by using them.**