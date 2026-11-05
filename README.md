*This project has been created as part of the 42 curriculum by xalves*

## Description

**NetPractice** is a networking project designed to introduce the fundamentals of networking and subnetting(dividing a single large network into smaller subnets). 

The project consists of 10 exercises, where small-scale simulated networks must be configured so that all devices can communicate with respective devices(or Internet) determined by the questions.

The goal of this project is to understand how TCP/IP addressing works and how devices such as computers, routers, and switches communicate within a network. It focuses more on concepts such as IP addresses, subnet masks and default gateway.

The project contains 10 levels, each of them is a different network configuration problem to be solved.

## Instructions

### Launching the Training Interface

First, download the NetPractice files provided on the project page and extract them into a folder.

Then there are 2 main ways of starting NetPractice from the extracted folder:

### **Option nº1 - (Just click it)**

You can open it by just simply double-clicking the `index.html` file in the folder.

That should open the NetPractice in your browser without creating a local web server.

### **Option nº2 - (./run.sh)**

From the folder, run in the terminal:

```bash
./run.sh
```

This command should start a local web server and opens NetPractice in your browser.

If the `run.sh` gives an error similar/or iqual to `permission denied: ./run.sh` just run a simple command:

```bash
chmod 777 run.sh
```

This will give `run.sh` all the permitions so it can me runned. 

Then just run the command `./run.sh` again.

### Using NetPractice

When the interface is open, you can enter your login to practice using your personal configuration.![Training_UI_example](image.png)

You can also use the **Evaluation** tab to generate a random network configuration suitable for evaluation.![Evaluation_UI_example](image-1.png)

The project contains 10 levels. Each level displays a network diagram with configuration fields that need to be adjusted.

For example level 6:

![level_6_example](image-2.png)

The objective is to modify the available fields until the network functions correctly.

The logs displayed at the bottom right inside a blue rectangle of the NetPractice interface can also help identify problems, such as invalid IP addresses or missing gateways.

At any time you have these buttons available to use:

* **Check again** — verifies whether the current configuration is correct.
* **Get my config** — exports the completed configuration for submission (although it is recomended you only do this once everything is corrected).

After successfully completing a level a button will appear to take you to the next level.

### Exporting Configurations

Before moving to the next level as mentioned before, make sure to export your configuration using the **Get my config** button.

Each completed level must have its own exported configuration file.

The exported files must be placed at the root of the Git repository.

### Submission

The project requires all 10 levels to be completed.

Please check the repository before submiting.

The repository must contain:

- README.md
- level1.conf
- level2.conf
- level3.conf
- level4.conf
- level5.conf
- level6.conf
- level7.conf
- level8.conf
- level9.conf
- level10.conf

## Resources

### Networking Concepts Studied

- **TCP/IP addressing** ==> system used to identify devices on a network (**IP** address identifies a device. **TCP/IP** defines how data is sent between devices)

- **Subnet masks** ==> determines which part represents the network and which part represents the host. (ex: 255.255.255.0 => [3 network & 1 host])

- **Default gateways** ==> device or a router, that a computer sends the data to when the destination is outside its local network. (imagine a switch case, and Default gateway is a default if no cases matches)

- **Routers** ==> devices that connects different networks and forward data between them.

- **Switches** ==> devices that connects multiple devices within the same local network (LAN)

- **OSI layers** ==> A 7 layered model used to understand how network communication works:
    1. **Physical** ==> Think of cables, signals, hardware
    2. **Data Link** ==> MAC addresses, switches
    3. **Network** ==> IP addresses, routers
    4. **Transport** ==> Controls how data is sent between applications and it makes sure it arrives correctly and in the right order.
    5. **Session** ==> Keeps track of a communication between two devices, from when it starts until it ends.
    6. **Presentation** ==> Data formatting/encryption
    7. **Application** ==> Protocols used by applications, such as HTTP and DNS


### Videos

- [NetworkChuck- You SUCK at Subnetting Youtube series](https://www.youtube.com/watch?v=5WfiTHiU4x8&list=PLIhvC56v63IKrRHh3gvZZBAGvsvOhwrRF)
- [Andrea Schauer- What Is a Default Gateway? | Simple Explanation for Beginners](https://youtu.be/TYlq7Si1SZc)

### Websites

- [Subnet Masks Table](https://www.connecteddots.online/resources/blog/subnet-masks-table)
- [TCP/IP Model vs OSI Model](https://www.fortinet.com/uk/resources/cyberglossary/tcp-ip-model-vs-osi-model)

## AI Usage

AI was used to help me understand/review/fortify some networking concepts that are required for the project, particularly TCP/IP and OSI models, subnet masks and default gateways.

AI was also used to help create a draft of this README and help with some orthographic errors.
