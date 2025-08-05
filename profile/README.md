<div align="left">
  <img width="225" height="263" alt="Logo" src="https://github.com/user-attachments/assets/d1786fed-47f8-46d7-9f73-bd421ed63ab8" />
</div>

# What Vispyr is

A one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration.

[High level Diagram]

# Prerequisites

The application to be instrumented and monitered must be running on an EC2 instance. 

# How to install

1. Clone our [CLI repository](https://github.com/Vispyr/vispyr-cli "Go to CLI page") and follow the instructions there to spin up Vispyr's backend in your AWS environment.
2. Copy the entire `vispyr_agent` folder to the root folder of your application.
3. Modify your `npm start` script to include `./deployAgent.sh`.
4. Re-run your application with these modifications made.
5. Access Vispyr's dashboard and watch your application's telemetry data through the URL generated in step 1.

# FAQ

# Learn more

For a more detailed and comprehensive description of Vispyr, along the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

