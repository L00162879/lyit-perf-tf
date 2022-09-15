# Terraform - Performance analysis and comparison of Infrastructure as Code (IaC) Tools (lyit-perf-tf)
The lab environment used for this research was built by following the best practices towards having a practical workbench that would allow the benchmark tests to be conducted in consideration of an impartial implementation, avoiding noise by external factors like variations in the network bandwidth external to the cloud platform, the use of a single command line interface for both implementation and the definition of the very same cloud services with the very same configurations.

## Test workbench
A representation of our benchmark workbench is below. Visual Studio Code was used to implement the Terraform and Bicep scripts. Then Azure Cloud Shell was used to execute the scripts. 
![Test workbench](/media/test-workbench.png)

## Azure cloud services
The following Azure cloud services have been specified and the respective scripts for both Terraform and Bicep have been implemented:

* Azure Application Insights (part of Azure Monitor)
* Azure Spring Apps – runtime environment for Java workloads, Kubernetes-based
* Azure Database for MySQL single server
* Azure Blob Storage

