# 🧹 Clean-Folder-HTML

PowerShell script to clean a specified folder and generate a styled HTML report summarizing the results.

## 📌 Features

- Deletes all files and subfolders in the specified directory
- Retries deletions up to 3 times with a configurable delay
- Logs deleted and skipped items
- Outputs a clean HTML report with:
  - Status (success or warning)
  - Deleted and skipped items
  - Full log of each attempt
- Lightweight and easy to configure

## 🖥️ Example Use Case

Clean up your Temp folder (`C:\Users\<YourName>\AppData\Local\Temp`) and get a report you can open in any browser.

## 🛠️ Configuration

Inside the script, you can customize:
```powershell
$targetPath   = "C:\Users\YourName\AppData\Local\Temp"
$maxRetries   = 3
$waitSeconds  = 15
$htmlReport   = "C:\Path\To\Your\Report.html"
