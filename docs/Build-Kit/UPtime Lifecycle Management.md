# UPtime Lifecycle Management

## 1.1 Purpose

Purpose of this document is to provide a plan for the management of UPtime throughout its full Product lifecycle.

## 1.2 Audience 

The primary audience for this guide is Product Ownership and Delivery / Run and Maintain Team Members.

## 1.3 Build Process

The Uptime development process can be found here https://confluence.dxc.com/display/MWH/Uptime+Development+Flow+and+Environment+Mapping

## 1.4 New Requirement Management

### 1.4.1 Intake Process

#### 1.4.1.1 Feature Requests

- New feature requests can be made through this form - [LINK](https://forms.office.com/Pages/ResponsePage.aspx?id=cTXzkw9Vz0Own80zEzjQhtD-dp9rFEpMtjnPn9yMoFRUMExEMENXR0YwVjQ3S0ZTV0NIWElXNEhFMi4u)
- Feature requests can be made by any stakeholder (e.g. Sales, Offering, Delivery etc.)
- All requests are added to a SharePoint List for review 
-    Weekly roadmap calls review the requests and analyze
-    Product Management and other Stakeholders review the requests
-    New features may be added to the backlog for immediate work or added to the longer-term Roadmap as a JIRA capability

#### 1.4.1.2  Bug Fix Requests

Bug fixes are identified in a number of ways:

-    Developer Unit testing
-    Testing team Unit and Integration testing
-    Customer issues
-    Product Owner reviews

Each of these are analyzed and one of the below actions is taken by the Product Owner:

- **Critical bug**
  - Generally raised through monitoring or by customer support teams
  - Triaged and identified for L3 support
  - Raised in JIRA and immediately assigned to a developer for work
- **Release Blocker/Issue**
  - Generally raised by testing teams running Integrations tests
  - Triaged by the PO and identified as a blocker to a release
  - Discussed and assigned to a developer for re-work in their existing Story/Task, or a new Task is created
  - Completed in line with release cycles
- **Known Issue**
  - Raised by anyone in the team
  - Triaged by the PO ad identified as a minor issue that doesn’t block the development cycle
  - Story is created and added to a future sprint/backlog
- **Cosmetic Issue**
  - Raised by anyone in the team
  - Triaged by the PO and identified as a cosmetic issue that requires review
  - Story is created and added to a future sprint/backlog

## 1.5  Release Management

### 1.5.1 Release Roles and Responsibilities

The following are the roles and responsibilities associated with release management.

Table 1: Release Management Roles and Responsibilities

| Role Name          | Responsibilities                                             |
| ------------------ | ------------------------------------------------------------ |
| Product Management | ◾ Identifies from the roadmap the high level  milestones for releases |
| Product Owner      | ◾ Identifies the JIRA Stories in a current  release and adds them to a JIRA Release<br />◾ Signs off the release after reviewing the  stories and accepting them<br />◾ Writes the release notes<br />◾ Communicates the release to stakeholders after  testing |
| DevOps Lead        | ◾ Creates a GitHub release based on the Stories identified by the PO<br/>◾ Pushes the release to a Test environment for testing<br/>◾ Pushes the release to QA after testing is  complete |
| Test Lead          | ◾ Signs the release off as successful for the PO  to communicate |
| Test Team          | ◾ Completes the Integration Testing                    |

### 1.5.2 Release Communications

Release communications are handled by the Product Owner to the relevant Stakeholders. The release communications include a set of Release Notes that describe what is in the release itself. 

Release notes from the build team will be for internal consumption. R&M/Account teams may need to adapt for customer consumption

A centralized location stores the numbered release notes alongside the Roadmap showing the forward Plan of Record and Plan of Intent for future capabilities.

> This doesn't exist today. Intention is to create going forward.

### 1.5.3 Release Structures

#### 1.5.3.1  Major Releases 

**Major Releases 2.0/3.0/4.0 etc will have a friendly name ‘alias’**

- 3.0 = Bernabeu (“UPtime Espressive Integration”)
- 4.0 = Wembley
- 5.0 = San Siro

Major functionality improvements (e.g. adding Espressive, PC Lifecycle) etc.

‘Kitchen English’ feature names listed in Roadmap

#### 1.5.3.2  Minor Release (3.1/3.2/3.3) etc

**Minor Release (3.1/3.2/3.3)** Odd numbers are bug fixes, security, hot fixes etc.

Even numbers are capability releases (e.g. 3.2 – Entitlements/Exceptions for PC Lifecyle Retail)

#### 1.5.3.3  Sprint Releases (22.3.1, 22.3.2)

- Sequential Agile sprint (Year.Month.Sequence)

- Fortnightly
- May or may not be included in Major/Minor release.

#### 1.5.3.4  Hot Fix Releases (##.#.#-HotFix)

- Created to apply hot-fixes to existing release branches

- Generally to apply immediate and urgent fixes


## 1.6  Deployment Guide
The deployment guide can be found in the Delivery Kit documentation here https://github.dxc.com/pages/WorkplaceAndMobility/DXC-MW-UPT/Delivery-Kit/.

It is recommended to keep all UPtime components up to date to ensure the maximum experience for the customer

## 1.7  Operations Guide

The Operations guide can be found here https://github.dxc.com/pages/WorkplaceAndMobility/DXC-MW-UPT/Delivery-Kit/Operations-Guide/

## 1.8  End-of-Life Strategy

#### 1.8.1.1  Customer offboarding Processes

<TBD by delivery/account team> - how does this process all start, what’s the engagement process.

> Engagement process to be defined by R&M Teams with accounts etc. - how does customer offboarding get initiated

#### 1.8.1.2  Technical decommissioning

##### 1.8.1.2.1    Azure decommissioning

Run and Maintain teams are to raise a request to the CloudOps team through PX ServiceNow. This request must include the details of the subscription and the request for the full decommissioning of the UPTime Azure Components.

##### 1.8.1.2.2    Boomi decommissioning

<TBD with Boomi team> - what’s the process for removing the sub-account.

> Still TBC with Boomi and Delivery teams - assume that sub-accounts can just be deleted

##### 1.8.1.2.3    Other offering services decommissioning

Decommissioning of other offerings that integrate with UPtime is in line with the Offering processes[[BH4\]](#_msocom_4) 

> Other offering procedures are to be taken into account
