<div align="left">
  <img width="225" height="263" alt="Logo" src="https://github.com/user-attachments/assets/d1786fed-47f8-46d7-9f73-bd421ed63ab8" />
</div>

# What Vispyr is

A one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration. By automating the deployment and configuration of our observability stack, we hope to introduce and facilitate the adoption of continuous profiling as an important complementary signal to metrics and traces.

Vispyr is composed of a backend and an agent. The [agent](https://github.com/Vispyr/vispyr-agent "Go to Vispyr agent") attaches to the application and generates telemetry data that is sent to [Vispyr's backend](https://github.com/Vispyr/vispyr-backend "Go to Vispyr backend"), which collects and stores this data while providing an easy-to-use dashboard where the user can see and correlate:
* CPU and Memory utilization
* P99 Latency metrics by application routes
* Flamegraph and table of continuous profiling data
* Scatterplot graph and table for distributed tracing
* A trace waterfall panel for analizing any selected trace

[High level Diagram]

*Vispyr currently supports only NodeJS applications*

# Prerequisites

The application to be instrumented and monitered must be running on an EC2 instance. 

# How to install

1. Clone our [CLI repository](https://github.com/Vispyr/vispyr-cli "Go to CLI page") and follow the instructions there to spin up Vispyr's backend in your AWS environment.
2. Copy the entire `vispyr_agent` folder to the root folder of your application.
3. Modify your `npm start` script to include `./deployAgent.sh`.
4. Re-run your application with these modifications made.
5. Access Vispyr's dashboard and watch your application's telemetry data through the URL generated in step 1.

# Learn more

For a more detailed and comprehensive description of Vispyr, along the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

