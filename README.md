# NetPractice

*This project has been created as a part of the 42 curriculum by alicigar.*

## Description

NetPractice is a practical introduction to computer networking. The goal is to solve 10 exercises by configuring simulated networks so that all devices can communicate with each other correctly.

To complete the exercises, you need to understand the following concepts:

To complete the exercises, you need to understand the following concepts:

- **IP address**: Every device on a network has a unique IP address; four numbers between 0 and 255 separated by dots (for example: 192.168.1.10)
- **Subnet mask**: Tells you which part of the IP identifies the network and which part identifies the device. Two devices can only communicate directly if they are on the same network (same mask, same IP range).

    | Mask | CIDR | Block size | Usable hosts | Range example |
    |---|---|---|---|---|
    | 255.255.255.0 | /24 | 256 IPs | 254 | .0 → .255 |
    | 255.255.255.128 | /25 | 128 IPs | 126 | .0 → .127 / .128 → .255 |
    | 255.255.255.192 | /26 | 64 IPs | 62 | .0 → .63 / .64 → .127 / ... |
    | 255.255.255.224 | /27 | 32 IPs | 30 | .0 → .31 / .32 → .63 / ... |
    | 255.255.255.240 | /28 | 16 IPs | 14 | .0 → .15 / .16 → .31 / ... |
    | 255.255.255.248 | /29 | 8 IPs | 6 | .0 → .7 / .8 → .15 / ... |
    | 255.255.255.252 | /30 | 4 IPs | 2 | .0 → .3 / .4 → .7 / ... |

- **Default gateway**: When a device wants to send data to another network, it doesn't know how to get there by itself. It passes the data to the gateway (the router's IP on its local network), which takes care of forwarding it.
- **Router**: A device that connects different networks together. It has one IP address per network it connects to, and uses a routing table to decide where to send each packet.
- **Switch**: A device that connects multiple devices within the same network. It does not need an IP address and does not separate networks — it just links devices together.
- **Routing table**: A list of rules that tells a device where to send packets. The **default** route (0.0.0.0/0) means "send everything you don't know where else to send to the gateway you put."
- **OSI model**: A 7-layer framework that standardizes how devices communicate over a network. This project focuses on _layer 2_ (switches, MAC addresses) and _layer 3_ (routers, IP addresses).

## Instructions

How to run the training interface:

-Download the .tgz from the project page and extract them into a folder of your choice.

Open a terminal in that folder and run:

    ./run.sh

Then, your browser will open automatically. 

If it doesn't, you can start the server manually:

    python3 -m http.server 49242

Then open your browser and navigate to http://localhost:49242

You may change the port number if needed (just make sure the URL matches the port you chose).

### How to use the interface:

- Enter your 42 intranet login in the field.

- Select **Training** to practice at your own pace, or **Evaluation** to generate a random configuration suitable for defense.

- Modify the white/unshaded fields to fix the network configuration.

- Click **Check again** to verify your solution.

- Once a level is completed, click **Get my config** to download your configuration file before moving to the next level.

### Submission requirements:

Complete all 10 levels and export one configuration file per level and place all 10 files at the root of your Git repository.

## Resources

The subject provided by 42 was used as a primary resource throughout the development process.

Additional external resources (such as tutorials and technical articles) were consulted to reinforce understanding and will be listed in this section:

Additional external resources (such as tutorials and technical articles) were consulted to reinforce understanding and will be listed in this section:

- TCP/IP adressing and OSI layers: https://www.geeksforgeeks.org/computer-networks/tcp-ip-model/
- Routers VS switches in a minute: https://www.cisco.com/site/us/en/learn/topics/small-business/network-switch-vs-router.html
- Subnet masks: https://www.youtube.com/watch?v=s_Ntt6eTn94&list=PLCXqoZAc8-tzD5N5oCyIyEcMg_NDs6o7C
- Default gateway explained in a minute in Spanish: https://www.youtube.com/shorts/RVxJoZM1jsQ
- A very useful NetPractice Tutorial: https://www.youtube.com/watch?v=pwjAyiscts8&t=94s

During the development of this project, AI was used as a learning support tool, mainly to:

-Clarify theoretical concepts related to networking, such as TCP/IP addressing, subnetting, routing tables, and the OSI model.
-Assist in writing and improving the project documentation.
-Help formulate questions and understand how the exercises work, without generating or copying solutions directly.

All AI-assisted content was reviewed, fully understood and validated, and all final design and implementation decisions were made consciously and responsibly. The project's code was entirely written and tested by me.
