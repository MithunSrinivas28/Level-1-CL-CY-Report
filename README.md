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

Application Layer: Directs user interactions, supporting applications like web browsers and email.

Presentation Layer: Translates and formats data; handles encryption and compression.

Session Layer: Manages and controls connections between devices.

Transport Layer: Ensures reliable data transfer, managing segmentation, and flow control.

Network Layer: Determines data routing across networks using logical addressing (e.g., IP).

Data Link Layer: Manages node-to-node data transfer within a network using MAC addresses.

Physical Layer: Handles the physical transmission of raw data (bits) via cables, radio waves, etc.


![380485123-0f215da3-5014-43d8-93f9-3755b32f2cfa](https://github.com/user-attachments/assets/13d4595c-dd18-47f5-93b0-60736a724b04)


 ###Simple example to learn OSI model:

A My device sends a frame across a physical network using Ethernet cables.
- The frame passes through various network devices, including:
    - Switch
    - Router
- The frame ultimately reaches the destination: uvcemarvel.com
- The server at uvcemarvel.com de-encapsulates the frame to extract the application data.
- The data includes a web request from a user (Mithun) who wants to view the homepage of uvcemarvel.com to apply project track
- The web server processes Mithun's request.
- The server encapsulates the information needed for the response into a new frame.
- The response frame is sent back through the network:
    - Switch
    - Router
- Finally, the response is received by Mithun.

# TASK 4:Encryption Techniques
The objective of the task was to learn about basic encryption and decryption using python.I learnt about Types of encryption techniques that is syymetric and asymmetric .I studied about AES AND RSA techniques .


# Symmetric Encryption

Symmetric encryption is a cryptographic method that uses the same key for both encryption and decryption. This key is shared between the sender and the recipient.

### Key Pair:

In symmetric encryption, there's only one key, which is shared between the sender and the recipient.


## AES (Advanced Encryption Standard)
It is a powerful encryption algorithm used to secure data by scrambling it in a way that only those with the correct key can decipher. Imagine it as a lock and key system for digital information
![Pasted image 20241016185351](https://github.com/user-attachments/assets/35551a65-7c85-4748-a3d7-88c0805a6be1)

Encryption Process: The AES algorithm processes the plaintext in multiple rounds (10 rounds for 128-bit keys). Each round consists of several operations:

SubBytes: Substitutes bytes using a predefined substitution table.
ShiftRows: Shifts rows of the state array to the left.
MixColumns: Mixes the data in each column.
AddRoundKey: Combines the state with the round key derived from the original key


# Asymmetric encryption:

Asymmetric encryption, also known as public-key cryptography, involves the use of two distinct but mathematically related keys: a public key and a private key.

### Key pair

The public key is shared openly and can be distributed to anyone who wants to send secure messages.

The private key is kept secret by the owner and is used to decrypt messages encrypted with the corresponding public key.

## RSA TECHNIQUES

RSA is a widely used asymmetric encryption algorithm. Here's a simplified breakdown of the process:

**1. Key Generation:**

- **Choose two large prime numbers:** These numbers should be kept secret.
- **Calculate the modulus:** Multiply the two prime numbers to get the modulus (n).
- **Calculate the totient:** Calculate the totient (φ(n)) of the modulus.
- **Choose an encryption exponent (e):** Choose a number (e) that is relatively prime to φ(n) and satisfies 1 < e < φ(n).
- **Calculate the decryption exponent (d):** Calculate the decryption exponent (d) such that (e * d) mod φ(n) = 1.


### WHY AES OVER RSA?:
AES is preferred over RSA for bulk data encryption due to its speed, efficiency, and ability to handle large datasets effectively. RSA is typically used for secure key exchange rather than for encrypting large amounts of data directly. In many secure systems, both AES and RSA are used together, with RSA handling key exchange and AES providing fast data encryption


![380485187-1eaae292-ced2-42c0-98bf-db50df8674c3](https://github.com/user-attachments/assets/d0f24530-8cc0-4027-b46f-c6fd7104e80b)
![380485214-083fbcbe-ce27-4dca-bd0a-5473432e87ef](https://github.com/user-attachments/assets/90a2cb95-eba5-4f97-b727-3e69df4673e5)  
![380485218-80da4388-2f35-4247-85e4-611eb3044f75](https://github.com/user-attachments/assets/7a58b0c3-6ce5-437f-b03e-077131da8b97)


# TASK 5:IP Addressing and Protocols
I learnt how to webscrape from a job website  using pyhton libraries such as beautifulsoup4 and pycrytodome where I could filter out the jobs according to my skills
I studied about the Ip address and protocols . I learnt how to analyze them and also about the subnets and NAT and how router plays the role in assigning the Ip address.

# What is IP address?
Every device connected to the internet has a unique address called an **Internet Protocol (IP) address**. This address helps computers communicate with each other. It's like a digital postal code.

**IP address structure:** 
    IP addresses are displayed as a set of four digits- the default address may be 192.158.1.38. Each number on the set  may range from 0 to 255. Therefore, the total IP address range ranges from          0.0.0.0 to 255.255.255.255.

  IP address is basically divided into two parts: X1. X2. X3. X4
          1. [X1. X2. X3] is the Network ID
          2. [X4] is the Host ID

##### YOUR ROUTER GIVES YOU THE IP ADDRESS
This is done through a protocol called **Dynamic Host Configuration Protocol (DHCP)**, which automatically assigns a local IP address (usually in the form of 192.168.x.x or 10.x.x.x) to devices on the local network.
When the device wants to access the network that is not in the same range (same street)
that's where default gateway aka router comes into play.

#### What is IANA?
The **Internet Assigned Numbers Authority (IANA)** is a key part of the global infrastructure that ensures the smooth functioning of the Internet

### Protocols

Think of protocols as the rules of the road for internet traffic. They define how data is formatted, transmitted, and received. Some common protocols include:
- **HTTP (Hypertext Transfer Protocol):** Used for transferring web pages.
- **TCP (Transmission Control Protocol):** Ensures reliable data delivery.
- **UDP (User Datagram Protocol):** Faster but less reliable than TCP, used for applications like streaming.
- **DNS (Domain Name System):** Converts human-readable domain names into IP addresses.



## Webscraping:

Web scraping is the process of extracting data from websites. It's like a digital librarian, collecting information from various online sources. For example, you might use a web scraper to gather product prices from different e-commerce websites.
Web scraping uses intelligence automation methods to get thousands or even millions of data sets in a smaller amount of time.

   **How does it work?**

1. **Request:** The scraper sends a request to the website, asking for the HTML code of a specific page.
2. **Parsing:** The scraper analyzes the HTML code to identify the data it wants to extract.  In the context of web scraping, parsing refers to the process of analyzing the HTML code of a web page to identify and extract the desired data.
4. **Extraction:** The scraper extracts the desired data, such as product names, prices, or descriptions.

SCRAPING IP ADDRESSES

![image](https://github.com/user-attachments/assets/b757b93d-be73-4bda-81da-1362d50fabf9)

WEBSCRAPING A WEBSITE
![380485650-d0f3e52f-1639-42ee-bc75-bda886977558](https://github.com/user-attachments/assets/1c801ac7-6ebb-4200-8ed8-9b2cc293619a)

# TASK 6: Kali linux and SSH
I got familiar with kali linux and Basic commands of Nmap.I learnt the importance of SSh and the types of penetration testing.I did scanning of of a target ip and found the open ports and their versions

## KALI Linux commands

### Sudo command 
  In **Kali Linux** (and other Linux distributions), the `sudo` (short for "superuser do") command allows a permitted user to execute a command as the **superuser** (root) or another user, as specified by the security policy. It is primarily used for administrative tasks that require higher privileges than a normal user account.
![Pasted image 20241023150909](https://github.com/user-attachments/assets/4813f710-c3ec-42a9-8040-cbc584c4774a)


Ping
`ping` command is a network utility used to test the **reachability** of a host on an IP network. It is commonly used to check if a particular system (device, server, or host) is online and responding to network requests.

![Pasted image 20241023162006](https://github.com/user-attachments/assets/a0bbddcb-3c45-4e1f-9fb5-ad33c79dc073)

  ### SN command

The `-sn` option is used to perform a **ping scan** (also known as a "no port scan"). When you use this option, Nmap disables the default port scanning phase and instead focuses on **host discovery**. It checks whether the hosts on the network are up (alive) without probing their open ports.
![Pasted image 20241023180758](https://github.com/user-attachments/assets/81e38c11-ff09-464e-b7fc-c8122d0c62c6)

Ping Scan (-sP): Discovers live hosts on a network by checking which IP addresses are active without scanning ports.

Stealth Scan (-sS): Performs a SYN scan, which is faster and less likely to be detected by firewalls compared to a full connection scan.

OS Detection (-O): Tries to determine the target’s operating system by analyzing network responses.

Specific Port Scan (-p): Targets specific port(s) on the host instead of scanning all commonly used ports.

Aggressive Scan (-A): Combines multiple scan types, including OS detection, version detection, script scanning, and traceroute.


## Penetration testing


Black Box Testing: The tester has no prior knowledge of the system. This simulates an external attack where the attacker has to discover vulnerabilities without any insider information.

White Box Testing: The tester has complete knowledge of the system, including source code and architecture. This allows for thorough testing and identification of vulnerabilities.

Gray Box Testing: The tester has partial knowledge of the system. This approach combines aspects of both black and white box testing, simulating an insider threat or a targeted attack.![Pasted image 20241023175132](https://github.com/user-attachments/assets/3d8e1d16-5ade-4067-83c6-2bc1e1c239e4)

In this screenshot it shows the ports and the and the type of the protocol running such as tcp etc.

## SSH

**SSH (Secure Shell)** is a network protocol that securely connects to remote systems. It encrypts data, ensuring that sensitive information like passwords stays protected during transmission.

### Why SSH Replaced Telnet

SSH replaced Telnet because Telnet transmits data, including passwords, in plain text, making it vulnerable to eavesdropping and attacks. SSH, in contrast, uses encryption to secure data, making it far more secure and suitable for managing remote systems.


# TASK 7: Databases

I learnt how mysql works and got a handle of the mysql workbench interface. I used thunderclient to connect from the vs code to the mysql workbench
I did some basic operations like create and read operations

# SSH

**SSH (Secure Shell)** is a network protocol that securely connects to remote systems. It encrypts data, ensuring that sensitive information like passwords stays protected during transmission.

### Why SSH Replaced Telnet

SSH replaced Telnet because Telnet transmits data, including passwords, in plain text, making it vulnerable to eavesdropping and attacks. SSH, in contrast, uses encryption to secure data, making it far more secure and suitable for managing remote systems.

# SSH

**SSH (Secure Shell)** is a network protocol that securely connects to remote systems. It encrypts data, ensuring that sensitive information like passwords stays protected during transmission.

### Why SSH Replaced Telnet

SSH replaced Telnet because Telnet transmits data, including passwords, in plain text, making it vulnerable to eavesdropping and attacks. SSH, in contrast, uses encryption to secure data, making it far more secure and suitable for managing remote systems.


![{1F35CE53-CA66-44F1-B6AF-84941E7FB7CE}](https://github.com/user-attachments/assets/c8058ccb-c1a4-48f7-967c-a37f7479a3e9)


![{CC399016-8E33-4DD3-8765-37E82134E4DA}](https://github.com/user-attachments/assets/ced9a57a-e874-44a5-92ce-8fb89a96d161)![{F713CB20-1C86-487A-8D95-5EF3E6BB4E08}](https://github.com/user-attachments/assets/2c26fb5c-3acd-4f88-988b-20207f729b33)
![Uploading {1F35CE53-CA66-44F1-B6AF-84941E7FB7CE}.png…]()





