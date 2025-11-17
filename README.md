# 🔒 Vulnerability Scanning and Fixing – Windows 11 (Insider Build)

## 📝 What I Did

- Installed **Nessus Essentials v10.10.1**
- Activated with a **free code**
- Scanned **my PC (10.31.187.41)** using unauthenticated mode

## 📊 First Scan Results

- Critical: 0  
- High: 0  
- Medium: 1 → TLS 1.0/1.1 advertised

## 🔧 Fix Applied

- Checked Microsoft docs and Tenable guides  
- Confirmed TLS 1.0/1.1 are disabled by default in Windows 11  
- Edited registry to stop TLS 1.0/1.1 from being advertised:
  - Added `Enabled = 0` and `DisabledByDefault = 1` for TLS 1.0 and TLS 1.1 (Client & Server)
- Rebooted PC

## 🔁 Second Scan Results

- Critical: 0  
- High: 0  
- Medium: 0 ✅

## 📁 Saved Files

- Exported **PDF report**
- Took **screenshots** of scan and registry changes
