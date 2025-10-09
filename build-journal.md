# Mini-SOC Build Journal

## Phase 1 - Environment Setup
- Created Azure account and accessed Azure Portal.
- Set up Resource Group: `MiniSOC-RG` in Australia East. The resource group is basically a folder that keeps all cloud related stuff together (LAW, Sentinel, VMs, etc)  
- Setup Log Analytics Workspace and added it to the Resource Group, this is a cloud database that will store all the logs
- Connected Microsoft Sentinel to the Mini-SOC LAW. Sentinel will monitor logs and also allow me to write write queries and build dashboards and alerts.

## Phase 2 - Log Ingestion

- Created a new resource (Virtual Machine), wouldn't let me continue unless I changed the free subscription type to "pay as you go"
- To ensure the Mini-SOC lab remains cost-controlled, I configured an Azure budget alert named Mini-SOC1 under my billing account.
Monthly Budget: USD $200
Alert Threshold: 80% (USD $160)
Email Notifications: Enabled at hugogibietis@gmail.com
This setup ensures proactive cost monitoring during continuous operation of Azure resources (Log Analytics Workspace, Sentinel, and virtual machines). It also demonstrates financial governance, a critical element of real-world SOC management and cloud security operations.
- After this I successfully deploy the Windows 11 Pro VM (MiniSOC-VM01) in Azure using the standard_B1s instance type -> configured trusted launch, secure boot and vTpm for security with diagnostics and auto shutdown enabled to support log ingestion into Microsoft Sentinel while keeping costs low.
- 





