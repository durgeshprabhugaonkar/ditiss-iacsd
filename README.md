Overview

This project demonstrates a basic reverse shell implementation in Python using socket programming and threading.
It is designed for educational purposes only, to help learners understand how client–server communication works at a low level and how reverse connections are established.

The project consists of two Python scripts:

server.py – Listens for incoming reverse shell connections and controls clients

client.py – Connects back to the server and executes system commands

Educational Objectives

This project helps in understanding:

Python socket programming

Client–server architecture

Reverse shell concepts

Threading and concurrency

Remote command execution

Handling multiple clients

Project Structure
.
├── server.py   # Reverse shell server (listener & controller)
├── client.py   # Reverse shell client (connects back to server)
└── README.md

How the Reverse Shell Works

The server starts and listens on a specific port.

The client initiates a connection back to the server (reverse connection).

The server accepts multiple clients using threading.

An interactive shell named turtle is used to control connected clients.

Commands entered on the server are sent to the selected client.

The client executes the commands on its operating system and returns:

1. Command output

2. Error output (if any)

3. Current working directory
