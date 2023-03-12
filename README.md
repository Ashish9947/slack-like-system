# slack-like-system

## Top level description of the proposed architecture

We want to design a real time messaging platform that allows teams to collaborate in a chat based interface.
I would propose a `Three-tier architecture`.
The components of the architecture are as follows:

- Front-end application (Presentation tier): This is the user-facing interface of the system that allows users to interact with the platform. It can be a web or a mobile application.

- Back-end server (App tier): This is the server-side of the system responsible for handling user authentication, message delivery, and other core functionalities. It typically includes a message broker that handles the exchange of messages between clients.

- Database (Data tier): The database is responsible for storing user information, channel data, and message history.

## Detailed description of each architecture element

- Front-end application:
The front-end application is the user interface that users interact with to send and receive messages. It can be a web or a mobile application that communicates with the back-end server through an API. The front-end application typically includes features such as user authentication, channel management, message composition, and notification settings. It also includes a real-time chat interface that displays messages and updates in real-time.

- Back-end server:
The back-end server is the core of the Slack-like system. It is responsible for handling user authentication, message delivery, and other core functionalities. The back-end server typically includes several components, such as:

 - Authentication and authorization: The back-end server authenticates users and manages access control to channels and conversations.
 - Message broker: The message broker is responsible for routing messages between clients. It manages message queues and ensures that messages are delivered in the correct order.
 - Presence service: The presence service tracks the online status of users and their availability for messaging.
 - API: The API exposes the functionality of the back-end server to the front-end application, allowing users to send and receive messages and perform other actions.
- Database:
The database stores user information, channel data, and message history. The database is typically divided into several tables, such as:
 - User table: The user table stores user account information, including user names, email addresses, and password hashes.
 - Channel table: The channel table stores information about channels, including their names and descriptions.
 - Message table: The message table stores the message history of each channel, including the message text, sender, and timestamp.
