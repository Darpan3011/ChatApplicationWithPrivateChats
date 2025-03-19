# Chat Application with Private Chats

This is a real-time chat application built using **Spring Boot** and **WebSockets**, enabling users to send **public** and **private messages**.

## Features 🚀
- Real-time messaging using WebSockets
- Private one-on-one chat functionality
- Group chat support
- STOMP protocol for WebSocket communication
- Simple front-end using HTML & JavaScript

## Technologies Used 🛠️
- **Spring Boot** (Java)
- **Spring WebSockets**
- **STOMP protocol**
- **Maven** (Build Tool)
- **HTML, JavaScript** (Frontend)
- **Thymeleaf** (For UI rendering)

---

## 📂 Project Structure
```
ChatApplicationWithPrivateChats
│── src/main/java/com/darpan/websocketwithprivate/
│   ├── WebSocketWithPrivateApplication.java  # Main Application
│   ├── config/WebSocketConfig.java  # WebSocket Configuration
│   ├── controller/MessageController.java  # Handles messaging
│   ├── model/Message.java  # Message DTO
│
│── src/main/resources/
│   ├── application.properties  # App configuration
│   ├── static/index.html  # Frontend (WebSocket client)
│
│── pom.xml  # Maven dependencies
│── mvnw, mvnw.cmd  # Maven Wrapper
│── .gitignore
```

---

## 🏗️ Setup Instructions

### 1️⃣ Prerequisites
Ensure you have the following installed:
- **Java 17+**
- **Maven**
- **Any IDE** (IntelliJ, Eclipse, VS Code)

### 2️⃣ Clone the repository
```bash
git clone https://github.com/Darpan3011/ChatApplicationWithPrivateChats.git
cd ChatApplicationWithPrivateChats
```

### 3️⃣ Run the application
Use Maven to build and start the application:
```bash
./mvnw spring-boot:run
```
OR (for Windows)
```bash
mvnw.cmd spring-boot:run
```

### 4️⃣ Access the Chat App
Once running, open your browser and go to:
```
http://localhost:8080
```

---

## 🔌 WebSocket Endpoints

| Endpoint              | Description |
|----------------------|------------|
| `/ws`               | WebSocket connection endpoint |
| `/app/chat`         | Send a public message |
| `/user/queue/messages` | Receive private messages |
| `/topic/public`     | Subscribe to public messages |

---

## 📝 How to Use
1. Open the application in a web browser (`http://localhost:8080`).
2. Enter a username and join the chat.
3. Send messages publicly or select a user for private messaging.
4. Messages will be delivered in real-time via WebSockets.

---

## 📜 License
This project is open-source and free to use.