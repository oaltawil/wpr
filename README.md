# Windows Performance Recorder

This repository contains a single PowerShell script "Start-WprCapture.ps1", which can be used to collect detailed debugging information about the operating system using the Windows Performance Recorder utility (wpr.exe). More specifically, the script runs WPR to capture CPU utilization, Disk I/O activity, File I/O activity, Registry activity, Network activity, and Mini-Filter Driver activity for 1 minute. WPR saves the generated event trace log file (.etl) in the folder specified by the "WprFolderPath" parameter.
