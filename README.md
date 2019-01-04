# WebSocket-SpringBoot | Getting Started

## Requirements

For building and running the application you need:
- [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [Maven](https://maven.apache.org)

## Build Application
You can build the application by using the maven build command like so:
```shell
mvn clean install -DskipTests
```

## Connecting to the WebSocket/ServerEndpoint
- After cloning the repo on your local machine, start the SpringBoot application.
- The application will be started on `http://localhost:8080/`. You can configure and start the application on a different post.
- The application will expose two endpoints.

  i. WebSocket (ws) Endpoint
  
  ii. HTTP Endpoint
 
- You need to establish a WS connection on `ws://localhost:8080/webSocket` with your websocket client.
- Once you establish a connection to the WebSocket endpoint, you will start listening to any messages that get broadcasted to the listeners.
 
## Broadcasting Messages to WebSocket Listeners
- To broadcast the message, you need to use the `http://localhost:8080/broadcast` endpoint.
- A query parameter `message` has been set up to broadcast messages.
- Make a HTTP `GET` or `POST` call on `http://localhost:8080/broadcast?message=Hello World`, and your socket listeners will receive the message `Hello World` on their clients.

## WebSocket Simple Client
You can also use this WebSocket Client. Download the `WebSocket-Client.zip` from [HERE](http://thegeekyasian.com/res/WebSocket-Client.zip).

## The Tutorial
If you want to learn how to create WebSocket in Spring Boot with the better understanding, you can check out a step-by-step tutorial on my blog [HERE](http://thegeekyasian.com/?p=13)
