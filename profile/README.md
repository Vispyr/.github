![Vispyr](https://raw.githubusercontent.com/vispyr/.github/main/profile/assets/logo.png)

<div align="left">
  <img width="1350" height="1575" alt="Image" src="https://github.com/user-attachments/assets/d1786fed-47f8-46d7-9f73-bd421ed63ab8" />
</div>

# What Vispyr is

A one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration.

[High level Diagram]

# Prerequisites

* The instrumented application must be running on an EC2 instance. 

# How to install

Download the CLI tools by cloning our [CLI repository](https://github.com/Vispyr/vispyr-cli "Go to CLI page") and follow the instructions there.

---
# I don't understand land
* Copy the entire `vispyr_agent` folder to the root folder of your application EC2 instance
* Modify your npm start script to include `./deployAgent.sh`
* Their app automatically sends telemetry to your observability backend

* Move folder to repo
* Misc (secrets management, existing TLS certs, etc)
* Push & deploy with CLI

---
# FAQ

# Learn more

For a more detailed and comprehensive description of Vispyr, along the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

