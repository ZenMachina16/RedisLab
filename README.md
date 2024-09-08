# RedisLab - Custom Redis Server

**RedisLab** is a custom Redis server implementation written in Go. This project is designed to provide a basic Redis-like key-value store functionality.

## Features

- Basic Redis-like commands: `SET`, `GET`, `HELLO`
- Built-in peer-to-peer communication
- Configurable server address

## Prerequisites

Before you start, ensure you have the following installed:

- **Go**: You can download and install Go from [the official Go website](https://golang.org/dl/). Ensure Go is properly set up by checking the version:
  ```bash
  go version

## Installation
This guide walks you through installing and setting up the RedisLab project.
Clone the Repository

```bash
git clone https://github.com/ZenMachina16/RedisLab.git
cd RedisLab

# Build the Project
Use the go build command to compile the project:

go build -o goredis main.go

# Running the Server

./main.go --listenAddr :5001

# Usage
# Once the server is running, you can interact with it using a Redis CLI or a similar client. The server supports basic commands:

# SET key value: Stores the value under the key.
# GET key: Retrieves the value associated with the key.
# HELLO: Returns a greeting from the server.

redis-cli -h <server-address> -p <port> SET mykey "myvalue"
redis-cli -h <server-address> -p <port> GET mykey
redis-cli -h <server-address> -p <port> HELLO
