# Overview

Vispyr is a one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration. By automating the deployment and configuration of the observability stack, we help facilitate the adoption of continuous profiling as an important observability signal, complementary to metrics and traces.

Vispyr is composed of a [backend](https://github.com/Vispyr/vispyr-backend "Go to Vispyr backend") and an agent. The agent attaches to the application and generates telemetry data that is sent to [Vispyr's backend](https://github.com/Vispyr/vispyr-backend "Go to Vispyr backend"), which collects and stores this data while provisioning an easy-to-use dashboard where the user can see and correlate:
* CPU and Memory utilization
* P99 Latency metrics by application routes
* Flamegraph and table of continuous profiling data
* Scatterplot graph and table for distributed tracing
* A trace waterfall panel for analyzing any selected trace

# Architecture
<div align="center">
  <img width="650" height="449" alt="Image" src="https://raw.githubusercontent.com/vispyr/.github/main/profile/assets/diagram.png" />
  ![Architecture Overview](https://github.com/user-attachments/assets/Basic_Architecture_dark_mode.svg)
</div>

  ![Architecture Overview](https://github.com/user-attachments/assets/Basic_Architecture_dark_mode.svg)

*Vispyr currently supports only NodeJS applications*

# Prerequisites

The application to be instrumented and monitored must be running on an EC2 instance. 

# Using Vispyr

* To deploy and teardown Vispyr in AWS, please use our [CLI](https://github.com/Vispyr/vispyr-cli "Go to CLI page").
* To see our observability stack and how its components are integrated, visit our [backend page](https://github.com/Vispyr/vispyr-backend "Go to backend page").
* For a demonstration of Vispyr's functionality in your local environment, we provide the [Demo App](https://github.com/Vispyr/vispyr-demo-app "Go to demo-app page").

# Learn more

For a more detailed and comprehensive description of Vispyr, along with the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

