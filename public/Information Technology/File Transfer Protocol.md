---
aliases:
  - FTP
---
# Overview 
File Transfer Protocol, is a standard network protocol used for the transfer of computer files between a client and server on a computer network. It was developed in the early 1970s and is one of the oldest protocols supported by the Internet, aside from [[Hypertext Transfer Protocol|HTTP]] and [[Simple Mail Transfer Protocol|SMTP]] .

## Functionality
FTP allows users to upload and download files, delete or rename files on a remote server, and navigate through the server's directory structure. 

## Mode of Operation
FTP operates on a client-server model. The client initiates a connection to the server and then the server responds to the client's request for file transfers and file management operation. 

There are two main modes of FTP
- Active FTP
	- The client connects from a random unprivileged port to the FTP server's command port (port 21). Then the server initiates the connection back to the client from its data port, port 20, to a client-specified port.
- Passive FTP
	- The client initiates both connections to the server, solving the problem of firewalls filtering the incoming data port connection to the client from the server.

## Security
Standard FTP does not encrypt its traffic; all transmissions are in clear text, including usernames, passwords, commands, and data. This can pose significant security risks, especially over unsecured networks. To address this, variants like [[File Transfer Protocol Secure|File Transfer Protocol Secure (FTPS)]], which extends [[File Transfer Protocol|FTP]] with [[Transport Layer Security]] (Transport Layer Security), and [[SSH File Transfer Protocol]] (SFTP), which uses [[Secure Shell|Secure Shell (SSH)]] to secure transfers, are used.

## Usage
FTP is widely used in environments where large files need to be transferred reliably and where the simplicity of the protocol is beneficial. It's commonly used in the fields of publishing, media transfer, software development, and in scenarios where large data repositories are accessed by a wide user base.

### Default Port
- Data Transfer: Port 20
- Command Control: Port 21
