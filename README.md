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
    
    - Push committed changes to a remote repository: `git push <remote>
    -  ![Pasted image 20241025225134](https://github.com/user-attachments/assets/a340a238-259a-4ca5-84fe-2f5ad203d945)
<branch>`



