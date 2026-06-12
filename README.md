# dev

PowerShell scripts for IT operations at Pharo Foundation, organised by function.

## Folders

### [dev/ASR](dev/ASR/)

Scripts for auditing Attack Surface Reduction (ASR) rule configurations on Windows endpoints.
Reads rule states via `Get-MpPreference` and maps each GUID to a human-readable name and mode.
No external dependencies — run elevated on any Windows 10/11 or Server 2016+ device.

### [dev/Microsoft Graph](dev/Microsoft%20Graph/)

Scripts for tenant reporting and administration via the Microsoft Graph API.
Covers Entra ID group exports, tenant snapshots, and M365 group cleanup using the Graph PowerShell SDK.
Requires appropriate Graph scopes (e.g. `Group.Read.All`, `Directory.Read.All`) and a browser sign-in prompt.

### [dev/Windows checks](dev/Windows%20checks/)

Scripts for spot-checking Windows device compliance and configuration.
Currently includes a Smart App Control status check to verify enforcement state on endpoints.
Intended for quick, ad-hoc health checks without deploying a full monitoring solution.
