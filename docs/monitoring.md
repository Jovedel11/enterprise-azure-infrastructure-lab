# Enterprise Azure Infrastructure Lab - Monitoring Phase

- In modern Azure you can simply monitor your compute service by navigating to Insights(Now Monitor) And can see now the Metrics and Logs but for Logs need to enable the Infrastructure monitoring to use it.

## Objective

- Create an Alert Rule for VM Availability Metric and to check the Metrics for VMs, both Linux and Windows and Metric it by category like Available Memory Bytes and ect.

## Monitoring Architecture

- For only in Project, It's enough to use Azure Monitor
- Check and Monitor each resources by the Insights Tab

## Design Decisions

- Create an Alert Rule that scope in RG for frontend and backend compute service
- Condition for the Resource Helth of that RG
- Monitor the Insights for Both VMs(Now is Monitor)
- Monitor in Metrics for scope in both VMs and the slected Metric

## Expected Learnings

- Can check each Resources Health
- What Metric and Logs different (By hands-on)
