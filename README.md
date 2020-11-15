# Windows Performance Recorder

This repository contains a single PowerShell script "Start-WprCapture.ps1", which can be used to collect detailed debugging information about the operating system using the [Windows Performance Recorder (WPR)](https://docs.microsoft.com/en-us/windows-hardware/test/wpt/windows-performance-recorder) utility. 

More specifically, the script runs WPR to capture the following type of information for exactly 1 minute:
- CPU utilization
- Disk I/O activity
- File I/O activity
- Registry activity
- Network activity
- Mini-Filter Driver activity

For more details on the type of information that can be collected by WPR, please visit: [Windows Performance Recorder Built-in Recording Profiles](https://docs.microsoft.com/en-us/windows-hardware/test/wpt/built-in-recording-profiles). 

WPR saves the generated event trace log file (.etl) in the folder specified by the "WprFolderPath" parameter (the .etl file name includes the computer name and date/time of capture).
