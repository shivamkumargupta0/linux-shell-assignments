#  Backup Directory Script

## Project Overview
This project contains a shell script named **`backup_directory.sh`** which is used to back up any directory in a Linux system.  
The script compresses the specified directory into a `.tar.gz` file and stores it inside a `backup_folder` directory located in the user’s home directory, along with a timestamp.

This tool is helpful for:
- Creating backups of important files and directories
- Automating backups using cron jobs
- Practicing Linux shell scripting and file handling


## Features
- Accepts a directory path as an argument
- Automatically creates a backup folder if it doesn’t exist
- Generates a compressed backup with timestamp
- Displays success confirmation with saved file path


##  Files Included
<table>
  <tr>
    <th>File Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>backup_directory.sh</td>
    <td>Main script used for creating backup</td>
  </tr>
  <tr>
    <td>README.md</td>
    <td>Documentation of the project</td>
  </tr>
</table>


##  How to Run the Script

### 1️ Give execution permissions
```bash
chmod +x backup_directory.sh

### Run the script
```bash
./backup_directory.sh <directory_path>


## Script Description
<table>
  <tr>
    <th>Component</th>
    <th>Explanation</th>
  </tr>
  <tr>
    <td><code>SOURCE_DIR="$1"</code></td>
    <td>Directory passed as argument</td>
  </tr>
  <tr>
    <td><code>BACKUP_DIR="$HOME/backup_folder"</code></td>
    <td>Backup storage location</td>
  </tr>
  <tr>
    <td><code>TIMESTAMP=$(date +"%Y-%m-%d_%H-%M-%S")</code></td>
    <td>Generates timestamp</td>
  </tr>
  <tr>
    <td><code>tar -czf</code></td>
    <td>Compresses folder to tar.gz</td>
  </tr>
  <tr>
    <td><code>mkdir -p</code></td>
    <td>Creates directory if it does not exist</td>
  </tr>
</table>


## Author
Shivam Kumar Gupta
Shell Scripting & Linux Enthusiast
