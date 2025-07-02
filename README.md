# CHAT-APPLICATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: Valina Veerendra

*INTERN ID*: CT04DF2540

*DOMAIN*: Full Stack Web Development

*DURATION*: 4 WEEEKS

*MENTOR*: NEELA SANTOSH

## 💬 WebSocket‑Chat (by Chiranjeevi325)

**Overview:**
A real-time group chat application built with **Socket.io** (WebSocket abstraction for Node.js) and **React**, styled with **Material‑UI** in a fun "The Walking Dead" theme ([github.com][1]).

### 🛠️ Key Features & Flow

* **Instant, bidirectional messaging** via Socket.io—clients connect and exchange messages in real-time.
* **Character selection**: users pick an avatar (character) before entering chatrooms.
* **Room management**: users can join/leave chatrooms; server tracks members and chat history.
* **Broadcasting**: a message sent by one user is relayed to all others in the same room.
* **Connection lifecycle**: users receive notifications when others connect or disconnect.
* **Frontend**: chat UI built with React and Material‑UI components ([forum.freecodecamp.org][2]).

### 📁 Typical Folder Structure

```
websocket-chat/
├── client/              # React app for chat interface
│   └── Chatroom.jsx     # Main component handling UI + socket logic
├── server/              # Node.js back end
│   ├── server.js        # Express + Socket.io server setup
│   └── handlers.js      # Event handlers for join, leave, message
├── public/              # Static assets served to browser
├── package.json         # Project scripts and dependencies
└── webpack.config.js    # Bundles React app for development
```



### ⚡ Setup & Run

```bash
npm install         # Install both server & client deps
npm run server      # Starts the Socket.io back end
npm run client      # Launches React dev server (typically at localhost:3001)
```



### 🔧 Technical Highlights

* **Server (Node.js + Socket.io)** handles:

  * New socket connections, disconnections
  * Events: `'select character'`, `'join room'`, `'leave room'`, `'message'`
  * Maintains `ClientManager` & `ChatroomManager` for user tracking and message history ([github.com][3], [itnext.io][4]).
* **Client (React)**:

  * Maintains socket in state, listens/emits events
  * `Chatroom.jsx` component updates UI based on events — users joining/leaving/send messages ([github.com][5]).
* **Modern JavaScript** (includes object-rest-spread); you need Node >=10 to avoid syntax errors ([github.com][3]).

---

### TL;DR:

This is a full-fledged, real-time group chat system using:

* **Socket.io** for server-client real-time communication,
* **React + Material-UI** for a responsive, themed UI,
* Modular Node.js server code handling rooms, users, and message broadcasts.

#output

![Image](https://github.com/user-attachments/assets/58108343-8e0e-43ca-ae60-5b694f41b1c6)
![Image](https://github.com/user-attachments/assets/eeb123ce-4cc5-429c-a223-9f91e202c384)
![Image](https://github.com/user-attachments/assets/1a48cc3b-6c99-481d-9717-79869c3cd5a9)
![Image](https://github.com/user-attachments/assets/60b94e6c-c482-42b7-9810-d7fc538e94b2)

