# What Vispyr is

A one-command solution to get continuous profiling and comprehensive monitoring for applications running on EC2 instances with proper network security and zero manual configuration. By automating the deployment and configuration of the observability stack, we help facilitate the adoption of continuous profiling as an important observability signal, complementary to metrics and traces.

Vispyr is composed of a [backend](https://github.com/Vispyr/vispyr-backend "Go to Vispyr backend") and an agent. The agent attaches to the application and generates telemetry data that is sent to [Vispyr's backend](https://github.com/Vispyr/vispyr-backend "Go to Vispyr backend"), which collects and stores this data while providing an easy-to-use dashboard where the user can see and correlate:
* CPU and Memory utilization
* P99 Latency metrics by application routes
* Flamegraph and table of continuous profiling data
* Scatterplot graph and table for distributed tracing
* A trace waterfall panel for analizing any selected trace

# Architecture
<div align="center">
  <img width="650" height="449" alt="Image" src="https://raw.githubusercontent.com/vispyr/.github/main/profile/assets/diagram.png" />
</div>


*Vispyr currently supports only NodeJS applications*

# Prerequisites

The application to be instrumented and monitored must be running on an EC2 instance. 

# How to use

### AWS deployment

Go to the [CLI repository]() page and follow the instructions under "Installation" section. Vispyr app will be deployed automatically on a newly created EC2 instance and a URL will be generated for accessing Vispyr's dashboard.

### Deletion

Go to the [CLI repository]() page and follow the instructions under "Teardown" section. Vispyr app will be destroyed and all infrastructe created will be eliminated.

### Demonstration

Go to the [Demo App repository]() page, clone it and run `docker compose up`.

# Learn more

For a more detailed and comprehensive description of Vispyr, along the motivation for its creation, please read our [case study](https://vispyr.com "Go to Case Study").

