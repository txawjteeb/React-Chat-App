## Chat Application built with ReactJS

Building the first part of the Socket.io Chat Application in ReactJS


### Updated: 10/18/2017
#### #React-Chat-App/src/server/SocketManager.js
This is the major component of which uses the Socket.io tool that emits and sends messages to either the Community Chatroom that I am building or the private chatroom based on the Chatroom Socket ID. This SocketManager will maintain, check, and verify users based on their Socket ID and connect it to similar Socket IDs.

The Socket Manager will also display users either joining, leaving, or disconnected in the chatroom.

#### #React-Chat-App/src/components/chats/ChatContainer.js
This is the second major component for each chatroom that is available. This sets that Active Chatroom and updates the status of the either the user typing, not typing, messages recieved, and messages sending.

The major functions of the ChatContainer.js is that it updates users of anyone typing and then updates anyone that is sending their message.

When the message is sent, the message is then appended or added onto the message container in the array in ReactJS' virtual DOM and re-renders quickly the whole message thread. But this is highly un-noticable because of ReactJS' Virtual DOM memory refresh speed.
