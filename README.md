# COSReports – Reporting Scripts Collection

This repository contains a growing collection of PowerShell reporting scripts focused on Microsoft 365 and Azure. These scripts are designed to help IT administrators and security professionals generate actionable insights and simplify auditing tasks.

Over time, the scripts may be consolidated into a PowerShell module for easier reuse and distribution.

---

##  Features

- Ready-to-use PowerShell reporting scripts  
- Enforced naming convention: **`Invoke-<ReportName>.ps1`** (e.g., `Invoke-AuthContextInventory.ps1`)  
- Focused on Microsoft cloud services (Entra, SharePoint Online, Teams, Conditional Access, Identity Governance, etc.)  
- Consistent output formats (e.g., formatted `.xlsx`)  
- Modular structure — new scripts will be added over time

---

##  Getting Started

### Prerequisites

- **PowerShell 7.x** (recommended)  
- Required modules per script (e.g., `Microsoft.Graph`, `ExchangeOnlineManagement`, `Microsoft.Online.SharePoint.PowerShell`, `ImportExcel`)  
- Appropriate Microsoft 365 permissions for running scripts

### Usage

1. Clone the repository:
```powershell
git clone https://github.com/Noble-Effeciency13/COSReports.git
```
2. Change into the `Scripts` directory.  
3. Choose a report script and review its comment-based help for prerequisites and usage.  
4. Run the report using its `Invoke-<ReportName>.ps1` script. For example:
```powershell
.\Invoke-AuthContextInventoryReport.ps1 -TenantName "contoso" -OutputPath "C:\Reports\"
```
5. Check the output in the specified folder.

---

##  Repository Structure

```
COSReports/
│
├── Scripts/
│   ├── Invoke-AuthContextInventoryReport.ps1  # Script to inventory auth-context assignments across M365
│   ├── Invoke-<FutureReport>.ps1
│   └── ...
│
└── README.md
```

---

##  Documentation

Each script includes:

- Comment-based help (`Get-Help .\Invoke-<ReportName>.ps1 -Full`)  
- Clear definitions of parameters, examples, and prerequisites  
- Output information (Excel, CSV, or console)

---

##  Disclaimer

These scripts are provided *as-is*, without warranty. Always test in a non-production environment before running in production.

---

##  Contributing

Contributions are welcome! To contribute:

1. **Fork** the repository  
2. Create a feature branch (e.g., `feature/invoke-newreport`)  
3. Add your script following the `Invoke-<ReportName>.ps1` naming convention, with comment-based help  
4. Submit a **pull request** with details about your script

---

##  Author

**Sebastian Flæng Markdanner**  
Website: https://chanceofsecurity.com