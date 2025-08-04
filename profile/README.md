# What Vispyr is

A one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration.

[High level Diagram]

# Learn more

For a more detailed and comprehensive description of Vispyr, along the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

# Prerequisites

* Application running on EC2. 
* AWS account and proper credentials (TBD).

# How to install

* Download the CLI tools by cloning our [CLI repository](https://github.com/Vispyr/vispyr-cli "Go to CLI page").
* Include a `.env` file in `vispyr-cli/` root folder with the fields:
```
AWS_ACCESS_KEY_ID
AWS_SECRET_ACCESS_KEY
AWS_REGION
PEER_VPC_ID
```
Where `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` are generated in the users section of AWS. `AWS_REGION` is your desired region to deploy, and `PEER_VPC_ID` is the VPC ID of your desired app to instrument.
* Run `npm install`.
* Run `npm run build && npm start -- deploy`

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
