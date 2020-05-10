# Azure Blueprint Tutorial

This repository contains source code for article published in Medium: [Secured & Consistent Landing Zone for Cloud Workload using Azure Blueprint](https://medium.com/marcus-tee-anytime/secured-consistent-landing-zone-for-cloud-workload-using-azure-blueprint-fbf7d07da379)

It contains 2 parts, which is ARM template, and Azure Policy template.

## Azure Resource Manager (ARM Template)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fguangying94%2FAzure-Blueprint-Tutorial%2Fmaster%2FARM%2520Template%2Fbastion.json)

This ARM template will deploy the following resources:

1. Azure Virtual Network
1. Network Security Group
1. Azure Virtual Machine - Windows Server
1. Azure Bastion
1. Azure Storage Account

Here's the architecture diagram:

![Diagram](/assets/diagram.png)

## Azure Policy

The folder contains the following Azure Policy template:

1. No Application Gateway in designated Azure Virtual Network
1. No Azure Firewall in designated Azure Virtual Network
1. No public IP address on all network interface card
1. Network Security Group to block direct internet inbound
1. Network Security Group to block direct internet outbound
1. Network Security Group to be presence in all subnets