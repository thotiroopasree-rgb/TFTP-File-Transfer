# TFTP – UDP-Based File Transfer System

## Project Overview
This project implements a TFTP-based file transfer application using C programming and Linux system programming. It follows a client-server architecture and uses UDP socket programming for communication between the client and server.

The application supports uploading files from the client to the server and downloading files from the server to the client.

## Technologies Used
C Programming, Linux, UDP Socket Programming, GCC Compiler, Linux System Calls, File Handling, and Client-Server Architecture.

## Features
- **File Upload (PUT):** Transfers files from the client to the server.
- **File Download (GET):** Downloads files from the server to the client.
- **UDP Communication:** Uses UDP sockets for network communication.
- **Packet Handling:** Uses RRQ, WRQ, DATA, ACK, and ERROR packet types.
- **Acknowledgement Handling:** Uses acknowledgements and retransmission attempts during data transfer.
- **Transfer Modes:** Supports different file transfer modes.

## Key Challenges
- Handling packet loss and communication issues in UDP, which does not guarantee packet delivery.
- Dividing files into smaller packets and maintaining the correct packet sequence.
- Managing communication between the client and server using socket programming.
- Handling file reading, writing, acknowledgements, and retransmission during file transfer.

## Project Structure

TFTP-File-Transfer/
├── main.c
├── client.c
├── server.c
├── mode.c
├── TFTP.h
└── README.md

## Compilation and Execution

### Compile the Client
```bash
gcc main.c client.c mode.c -o client
```

### Compile the Server
```bash
gcc server.c mode.c -o server
```

### Run the Server
```bash
./server
```

### Run the Client
Open another terminal and execute:
```bash
./client
```

## Learning Outcomes
- Practical understanding of C programming and Linux system calls.
- Experience with UDP socket programming.
- Understanding of client-server communication.
- Hands-on experience with file handling and packet management.
- Improved debugging and problem-solving skills.
