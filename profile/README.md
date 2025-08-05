![Vispyr](https://raw.githubusercontent.com/vispyr/.github/main/profile/assets/logo.svg)

<div align="left">
  <img src="https://raw.githubusercontent.com/vispyr/.github/main/profile/assets/logo.svg" alt="Organization Logo" width="200"/>
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

