| [Home](../README.md) |
| -------------------- |

# Contents

The **USB Management Exceptions** solution pack contains the following resources.

## Dashboards 

| Name                                      | Description                                                                                                                                                                            |
|:------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| USB Approval System                       | Displays USB Request Status and USB Request Status (Validation)                                                                                                                        |
## Connectors

| Name                                    | Description                                                                                                                                         |
|:----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| Fortinet FortiEDR                       | FortiEDR Connetor to Move Collectors from Current Group to allow USB Group.                                                                         |
| Microsoft Exchange                      | Microsoft Exchange connector fetches Request and approval by Email.                                                                                 |
| Microsoft Active Directory              | Microsoft Active Directory Connector to get requester information and Manager details.                                                              |



## Module Schema

| Name         | Description                                                                                  |
|:-------------|:---------------------------------------------------------------------------------------------|
| USBs         | A module contains Requester Name,Requester Username, Requester Email, Manager Name, Manager Email, Machine Name , Request Status , Manager Justification, Manager Approval Status, Allowed Until and  Validation Status|


## Picklists

| Name                                   |
|:---------------------------------------|
| ApprovalStatus                         |
| USBUSerRequest                         |
| ValidationRequest                      |
| StatusApproval                         |
| Status                                 |


## Schedules

| Name                                                                 | Description                                                                                   |
|:---------------------------------------------------------------------|:----------------------------------------------------------------------------------------------|
| Remove USB Permission                                                | This schedule is triggered every 5 minutes to revoke USB Access                               |


## Playbook Collection

| USB Approval system                   |
| :------------------------------------ |


| Playbook Name                                              | Description                                                                                 |
|:-----------------------------------------------------------|:--------------------------------------------------------------------------------------------|
| USB Exception                                              | This playbook to give USB Access to Machine                                                 |
| Remove USB Permission                                      | This playbook to revoke USB Access from Machine after the status become expire              |
| Validation Moving                                          | This playbook to validate if the operation succeeded                                        |


>**WARNING:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.

# Next Steps

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
|-----------------------------------------|-------------------------------------------|---------------------|
