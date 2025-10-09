# Mini-SOC Build Journal

## Phase 1 - Environment Setup
- Created Azure account and accessed Azure Portal.
- Set up Resource Group: `MiniSOC-RG` in Australia East. The resource group is basically a folder that keeps all cloud related stuff together (LAW, Sentinel, VMs, etc)  
- Setup Log Analytics Workspace and added it to the Resource Group, this is a cloud database that will store all the logs
- Connected Microsoft Sentinel to the Mini-SOC LAW. Sentinel will monitor logs and also allow me to write write queries and build dashboards and alerts.

--

## Phase 2 - Log Ingestion

