# Terraform - Performance analysis and comparison of Infrastructure as Code (IaC) Tools (lyit-perf-tf)
The lab environment used for this research was built by following the best practices towards having a practical workbench that would allow the benchmark tests to be conducted in consideration of an impartial implementation, avoiding noise by external factors like variations in the network bandwidth external to the cloud platform, the use of a single command line interface for both implementation and the definition of the very same cloud services with the very same configurations.

## Test workbench
A representation of our benchmark workbench is below. Visual Studio Code was used to implement the Terraform and Bicep scripts. Then Azure Cloud Shell was used to execute the scripts.
<p align="center">
  <img alt ="Test workbench" width="275" height="175" src="/media/test-workbench.png">
</p>

## Azure cloud services
The following Azure cloud services have been specified and the respective scripts for both Terraform and Bicep have been implemented:

* Azure Application Insights (part of Azure Monitor)
* Azure Spring Apps – runtime environment for Java workloads, Kubernetes-based
* Azure Database for MySQL single server
* Azure Blob Storage

Azure Spring Cloud runtime, one Azure storage account, one MySQL server, and one Azure App Insights component was used for all the scenarios with both IaC tools. The services for both Terraform and Biceps are below. 

<p align="center">
  <img alt ="Azure Services – Terraform definitions" src="/media/azure-services-tf-definitions.png">
</p>

## Command line interface
The executions were controlled and timed with Powershell and the Measure-Command cmdlet. A cmdlet is a lightweight command used in the PowerShell environment. Such strategy also provided an impartial way of starting the execution scripts for Terraform and Bicep.

<p align="center">
  <img alt ="Azure Services – Terraform definitions" src="/media/lyit-perf-tf-RUNNING.png">
</p>