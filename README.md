# Level-1-CL-CY-Report
Report for level 1 tasks 

# Task 1: Linux Based Task with Socket.io

The goal was to learn about websockets and create a chat application using node js
I learnt about websockets in general and how they are responsible for building effienct chat systems.I was also introduced to Node.js and Express.js and the differnt methods of creating a chat app.
I also built a real time chat app ith HTML and express.js
## What is Socket io?

**Socket.IO** is a JavaScript library that enables real-time, bidirectional communication between a web server and clients (browsers or mobile apps). It's built on top of WebSocket technology, providing a more robust and flexible way to handle real-time events compared to traditional HTTP polling.
![image](https://github.com/user-attachments/assets/b832cbab-5c1e-4b77-ab24-bcf08060a70a)


#### What is the problem with polling??
With HTTP polling, the client constantly sends requests to the server asking for updates. This can be inefficient, wasting bandwidth and server resources on unnecessary communication
- As the number of clients increases, the server load can become overwhelming due to the constant polling requests
So Socket io was introduced

### Express.js over node.js
Express.js is better than plain Node.js for web development because it simplifies routing, request handling, and middleware management, improving code organization

#### CORS in WebSockets: A Brief Overview

**CORS (Cross-Origin Resource Sharing)** is a mechanism that allows a web page to make requests to a server on a different domain than the one that served the web page. While CORS is primarily used for HTTP requests, it also plays a role in WebSockets.

![380484168-5ba1c2f4-41a8-440b-a98c-c25d0e356bd6](https://github.com/user-attachments/assets/a5cf827a-06fb-4166-a8cd-f5c16b471e98)

![380484291-040f57b3-4701-4343-9cfe-ba985d660e77](https://github.com/user-attachments/assets/8840e5d3-5590-4159-a9a7-876244c096d4)



# TASK 2:Git Bash and GitHub

I got familiar with basic git commands while using git bash.I learnt how to create repository and add files into them.I then learnt how to commit changes and initaie pull request to repository.I also learnt about branching and merging 

## Understanding Git and Git Bash

**Git** is a distributed version control system that tracks changes in files over time. It allows you to collaborate effectively with others on projects, manage different versions of your code, and revert to previous states if necessary.
(It can related to a bank account statements where all the credit and debit changes made in the bank account are tracked in the passbook)


**Git Bash** is a command-line interface specifically designed for Git. It provides a convenient way to interact with Git repositories and execute Git commands.


## Basic Git Commands

#### Some basic definitions using the command  "git help"

![Pasted image 20241025222229](https://github.com/user-attachments/assets/a70d2e8d-23da-4de3-8de6-0b41ed8e0754)


1. **`git help`**: Provides documentation for any Git command.
2. **`mkdir`**: Creates a new directory.
3. **`cd`**: Changes the current directory.
4. **`ls`**: Lists files and directories.
5. **`git config --global user.name "<name>"`**: Sets a global Git username.
6. **`whoami`**: Shows the current user’s username.
7. **`pwd`**: Displays the current directory path.
8. **`ls -l`**: Lists files with detailed information.
9. **`git add`**: Stages files for commit.
10. **`git commit`**: Saves staged changes to the repository.
11. **Creating repository in Git Bash vs. GitHub**:

- **Git Bash**: Initializes a local repository.
- **GitHub**: Hosts a remote repository for collaboration.

- 12. **Initialization:**
    
    - Create a new Git repository: `git init`
    - Clone an existing repository: `git clone <repository URL>`
13. **Staging Changes:**
    
    - Add files to the staging area: `git add <filename>`
    - Add all modified files: `git add .`
14. **Committing Changes:**
    
    - Commit staged changes to the local repository: `git commit -m "Commit message"`
15. **Pushing Changes:**
    
    - Push committed changes to a remote repository: `git push <remote><branch>`

    A snippet of the gitbash terminal you can make changes in your change repository 
    -  ![Pasted image 20241025225134](https://github.com/user-attachments/assets/a340a238-259a-4ca5-84fe-2f5ad203d945)



# TASK 3:OSI MODEL

I learnt about the OSI model and how it works.I made the detail flowchart of osi model using draw.io

## What is OSI model?
The Open Systems Interconnection (OSI) model is a conceptual framework that divides the communication process between computers into seven layers. Each layer handles a specific aspect of the communication, from the physical transmission of bits to the application-level protocols.

. Physical Layer:**

- Handles the physical transmission of bits over a physical medium (e.g., cables, optical fibers, wireless).
- Concerned with electrical, mechanical, and procedural aspects of communication.
- Examples: Ethernet, Wi-Fi, Bluetooth

**2. Data Link Layer:**(Frame)

- Responsible for framing data into packets and ensuring reliable transmission across a physical link.
- Handles error detection and correction, flow control, and multiplexing.
- Examples: PPP, Ethernet, ATM

**3. Network Layer:**(packet)

- Handles the routing of data packets across networks.
- Responsible for addressing, routing, and packet switching.
- Examples: IP (Internet Protocol), IPv6, ICMP (Internet Control Message Protocol)

**4. Transport Layer:**(Segment)

- Provides reliable end-to-end communication between applications.
- Handles flow control, error control, and multiplexing.
- Examples: TCP (Transmission Control Protocol), UDP (User Datagram Protocol)

**5. Session Layer:**

- Manages sessions between applications.
- Handles synchronization, checkpointing, and dialog control.
- Examples: RPC (Remote Procedure Call), NFS (Network File System)

**6. Presentation Layer:**

- Handles the presentation of data, including encryption, compression, and syntax conversion.
- Ensures that data is in a format that can be understood by the application.
- Examples: JPEG, MPEG, ASCII

**7. Application Layer:**

- Provides services to applications, such as file transfer, email, and web browsing.
- Interacts directly with user applications.
- Examples: HTTP (Hypertext Transfer Protocol), FTP (File Transfer Protocol), SMTP (Simple Mail Transfer Protocol)
![380485123-0f215da3-5014-43d8-93f9-3755b32f2cfa](https://github.com/user-attachments/assets/13d4595c-dd18-47f5-93b0-60736a724b04)


 Simple example to learn OSI model:

A device sends a frame across a physical network using Ethernet cables.
- The frame passes through various network devices, including:
    - Switch
    - Router
    - Another switch
- The frame ultimately reaches the destination: networkchuck.coffee.
- The server at networkchuck.coffee de-encapsulates the frame to extract the application data.
- The data includes a web request from a user (Johnny) who wants to view the homepage of networkchuck.coffee to shop for coffee.
- The web server processes Johnny's request.
- The server encapsulates the information needed for the response into a new frame.
- The response frame is sent back through the network:
    - Switch
    - Router
    - Switch
- Finally, the response is received by Johnny.
