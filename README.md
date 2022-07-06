# Log-Analytics-Overview


# Log Analytics - Get Schema
- Before working through logs, it's important to understand the data types within each column.
- Use the 'getschema' command to view the data types of each column.
- Values can be a string or day/time value


<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177388161-bb372279-f34d-43e5-9810-aee78411c550.png" height="95%" width="95%" alt="LAW"/>

<p/>



# Log Analytics - Queries based on time
- Here users can view administrative activites performed such as deleting virtual machines and groups
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177389757-40340920-a16c-4e45-942e-ca39bfc06828.png" height="95%" width="95%" alt="LAW"/>

<p/>

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177390232-3c55d7aa-be47-4165-8375-8285013636c2.png" height="95%" width="95%" alt="LAW"/>

<p/>




# Log Analytics - Filterting for Data

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177443878-310240d7-9e59-4bc6-9a8d-f4168cfe2a2c.png" height="95%" width="95%" alt="LAW"/>

<p/>


# Log Analytics - Projection and Dynamic Data Types
- When we want to to view the AzureActivity log, we enter AzureActivity in as a KQL
- It will show a variety of columns but what if we want to display only a select few
- Users can also project and manipulate columns of Dynamic Data types
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177444308-8c1fdd48-efd7-4351-90dc-7862c19c6d5f.png" height="95%" width="95%" alt="LAW"/>

<p/>

# Project only three columns in this log
- This will project/show only specific columns we want to be shown
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177446858-1dd35cc8-e50a-437e-824a-442d09ebeadb.png" height="55%" width="55%" alt="LAW"/>

<p/>


# Log Analytics - Exploring the sign-in logs table 
- Remember that in order to work with Strings, you have to convert it to a dynamic data type. 
- To convert it to a dynamic data type, 
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177450765-87e7112e-b133-4baf-83e5-d7564d385128.png" height="55%" width="55%" alt="LAW"/>

<p/>

# This shows the failed sign ins
- Error code of 0 means that there was a successful sign in.
- These codes a failed sign-ins.
- It also shows the reason of the failed sign-ins under status
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177450771-7e8d4cdf-2e4e-4080-afbe-c0037644c298.png" height="125%" width="125%" alt="LAW"/>

<p/>


# Exploring the Azure Firewall Logs
- AzureDiagnostics log is Azure Firewall
- The AzureFirewall resource is streaming data to Sentinel via the LAW. 
- Multiple resources can so ensure that when you are running AzureDiagnosts logs, filter for the resource "Azure Firewall"
- In this example, we only enabled diagnostics for Azure Firewall


# Some data types are just a string but what if we want to collect specific data within the string?
- We can parse the string
- View video #213 on Udemy



# Log Analytics Workspace - Security Events
- Security Event table gets created when an event is created in Windows Event Viewer 
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177461672-8eb46252-14b0-49c2-adc9-9251685af9ce.png" height="125%" width="125%" alt="LAW"/>

<p/>


