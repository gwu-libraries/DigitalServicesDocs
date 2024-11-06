---
layout: page
title: "Audit Tool"
permalink: /managing/audittool/
---
# **This tool has been depreciated!** 

# Audit Tool
[Github Repo](https://github.com/gwu-libraries/audit-tool)

The Simple Audit Tool is a command-line tool designed to inventory and monitor file changes (additions, alterations, and deletions) on a storage filesystem. 

## Functionality
- Analyzes for and keeps a log of all changes detected (additions, alterations, deletions)
- Change reports can be automatically emailed to staff.
- Requests humans manually review that all changes were deliberate, non-malicious, and complete. If approved, inventory is updated with changes.
- In combination with cron jobs, can run scheduled audits.

*What the tool does not do:*

- Audit files before and after data exchange (i.e., when adding files to storage). That must happen using other tools (e.g., rsync, bagit).

## Approving Weekly Change Logs - gwspec-digcol1
This is assuming you've reviewed the weekly logs and found no issues.
- Log into gwspec-digcol1
- Change directory to audit-tool directory and activate environment
```
     cd /opt/audit-tool 
     source ENV/bin/activate
```
- Add changes to the canonical inventory by linking to the JSON report
````
python audit_tool.py update /path to json report
````

