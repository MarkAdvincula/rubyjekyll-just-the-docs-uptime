---
layout: default
title: Install and Configuration Guide
parent: Delivery Kit
has_children: true
permalink: "/docs/Delivery-kit/Install and Configuration Guide"
---

# Pre-Requisites

## <b> 01 Azure Prerequisites</b>
- Azure DevOps organisation with a paid tier Microsoft-hosted agent as the initial terraform may exceed the free tier time limit
- Azure DevOps Terraform and File Creator Extensions
- Azure AD account with access rights to Azure DevOps and rights to configure a Service Principle with Contribute Permission on Subscription
- Infrastructure: https://github.dxc.com/Uptime/terraform/tree/master/cps 
- GitHub Enterprise to link on AzureDevOps (Terraform, Deployment pipelines)
- GitHub PAT (Personal Access Token) with rights to create a GitHub Enterprise Server service connection to https://github.dxc.com
- SonarQube installed in order to test code quality for backend APIs

## <b>02 Repositories Prerequisites</b>

  Frontend:
  > - https://github.dxc.com/Uptime/Uptime-storybook
  > - https://github.dxc.com/Uptime/portal-web

  Backend:
  > - https://github.dxc.com/MWA/ms-uptime-base-api
  > - https://github.dxc.com/MWA/ms-asset-api
  > - https://github.dxc.com/MWA/ms-user-api
  > - https://github.dxc.com/MWA/ms-order-api
  > - https://github.dxc.com/MWA/ms-incident-api
  > - https://github.dxc.com/MWA/ms-shipping-api
  > - https://github.dxc.com/MWA/ms-knowledge-api

## <b> 03 OKTA Prerequisites</b>
* Frontend deployed in Azure DevOps pipeline
* Make sure that Client ID, and base_url are already available. Client ID, and base_url should be provided once an OKTA app is created. These will be used as a configuration in one of the releases.
* Logo file is obtained, stored in Okta system, and URL to logo is known.

## <b> 04 ServiceNow Prerequisites </b>
* Existing working ServiceNow instance
* ServiceNow Password
* ServiceNow URL
* ServiceNow USER

## <b> 06 Boomi Prerequisites </b>

* Boomi credentials
* Boomi URL

## <b> 07 ASD Chat Prerequisites </b>

* Deployed azure webapp for ASD CCL and edit config in here
https://github.dxc.com/ModernWorkplace/FASD_Connect_Chat/blob/master/BotConnector/Configuration.json to point the correct ServiceNow

Please refer to this document for UPtime installation prerequisites:

[Pre-Requisites](https://confluence.dxc.com/display/MWH/Pre-Requisites)