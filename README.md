# Full Stack Chat App

A real-time chat application built using **Spring Boot**, **WebSocket**, **STOMP**, HTML, CSS, and JavaScript. This application enables users to exchange messages instantly through a WebSocket connection.

## Features

* Real-time messaging using WebSocket
* STOMP messaging protocol support
* Spring Boot backend
* Simple and responsive chat interface
* Broadcast messages to all connected users
* Easy setup and deployment

## Tech Stack

### Backend

* Java
* Spring Boot
* Spring WebSocket
* STOMP Messaging

### Frontend

* HTML
* CSS
* JavaScript

### Build Tool

* Maven

## Project Structure

```text
src/
├── main/
│   ├── java/
│   │   └── com/chat/
│   │       ├── ChatappApplication.java
│   │       ├── config/
│   │       │   └── WebSocketConfig.java
│   │       ├── controller/
│   │       │   └── ChatController.java
│   │       └── model/
│   │           └── ChatMessage.java
│   └── resources/
│       ├── application.properties
│       └── templates/
│           └── chat.html
└── test/
    └── java/
        └── com/chat/
            └── ChatappApplicationTests.java
```

## How It Works

1. A user opens the chat page.
2. The frontend establishes a WebSocket connection with the Spring Boot server.
3. Messages are sent using STOMP endpoints.
4. The server receives the message and broadcasts it to all subscribed clients.
5. Connected users instantly receive the new message.

## Prerequisites

* Java 17 or later
* Maven 3.8+
* Git

## Installation

### Clone the Repository

```bash
git clone https://github.com/PrachiMadhukarPatil12345/Full-Stack-Chat-App.git
cd Full-Stack-Chat-App
```

### Build the Project

```bash
mvn clean install
```

### Run the Application

```bash
mvn spring-boot:run
```

or

```bash
java -jar target/chatapp.jar
```

## Access the Application

Open your browser and visit:

```text
http://localhost:8080
```

## WebSocket Endpoints

### Connection Endpoint

```text
/ws
```

### Publish Message

```text
/app/sendMessage
```

### Subscribe for Messages

text
/topic/messages

## Author

Prachi Patil


