# Deploy a high-availability web app using CloudFormation (Udacity Project 2)
This project consists of two parts:

1. **Diagram:** To develop a diagram that presents a visual aid the understanding of CloudFormation script.

2. **Script (Template and Parameters):** To interpret and create a matching CloudFormation script.


## Diagram

This was built using **[Lucid Chart](https://www.lucidchart.com)**

![image](https://user-images.githubusercontent.com/18303044/182663625-1afde65d-f307-4d6d-ac24-5f0ca491a0b7.png)


## Infrastructure as Code (IAC)

Run the below on the terminal to create the network infrastructure
```bash
./create.sh demoinfra infra.yml infra-parameters.json 
```

Run the below on the terminal to create the server infrastructure
```bash
./create.sh demoserver servers.yml servers-parameters.json 
```

To update any of the above created infrastructure, run the below on the terminal
```bash
./update.sh <<stack-name>> <<template-body file>> <<parameters file>>
```

To delete any of the above created infrastructure, run the below on the terminal
```bash
./delete.sh <<stack-name>> <<template-body file>> <<parameters file>>
```
