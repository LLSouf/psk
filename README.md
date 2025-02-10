# Process Memory Killer 🔍💥

An interactive Bash script for monitoring and managing process memory usage with kill capabilities. 🖥️💣

## Features ✨
- 📊 Memory usage display in MB
- 🔎 Process filtering by name pattern
- ☠️ Bulk termination of matching processes
- 🔄 Interactive search/kill loop
- 📋 Tabular formatted output
- 🎯 Case-insensitive search

## Prerequisites ⚙️
Requires standard Unix tools:
ps, grep, awk, kill
Tested on Linux/Bash

## Installation 📥
```bash
git clone https://github.com/LLSouf/psk/
cd psk
chmod +x psk
```
## Usage 🚀
```bash
./psk app_name_1 app_name_2 ...
```
## Workflow 🔄
Initial Search:

```bash
./psk.sh chrome firefox
```
Output:
```bash
Process              Memory Usage (MB)
chrome                452.32 MB
firefox               387.91 MB
```
Interactive Menu:
```bash
[a : Kill all]    [any other search for other apps] :
```
a → Kill all listed processes
other  → New search term(s)

## Safety Considerations ⚠️
❗ Data Loss Risk: Killing processes may cause unsaved work loss
🔐 Requires user confirmation before termination
⚠️ Test first without a option to verify matches

## Troubleshooting 🚨
No Processes Found:
Verify process names with ps aux

## Permission Denied:
Run with sudo for system processes

## Ghost Processes:
Use kill -9 manually if needed
