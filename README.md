# Linux System Management Assignment

This repository contains the results of a Linux system and network management assignment, executed using Windows Subsystem for Linux (WSL).

## Overview of Tasks
This project demonstrates proficiency in basic Linux command-line operations across four main areas:

* **Part 1: System Management:** Created directories and captured system information (`uname -a`) and memory usage (`free -m`) into `system.txt`.
* **Part 2: Process Management:** Demonstrated starting background processes (`sleep`), listing them (`jobs`, `ps aux`), and terminating them (`kill`).
* **Part 3: Network Commands:** Tested external connectivity (`ping`), checked local IP configurations (`ip a`), and monitored open ports (`ss -tuln`), saving network details to `network.txt`.
* **Part 4: Version Control:** Initialized a local Git repository and successfully pushed the project to GitHub using a Personal Access Token (PAT).

## Technologies Used
* Ubuntu (via WSL 2)
* Git & GitHub
* Bash Scripting / Command Line Interface
# Linux System and Network Management Assignment

This repository contains the completion of a multi-part Linux system management assignment. All tasks were executed using the command-line interface via Windows Subsystem for Linux (WSL).

## 🚀 Project Overview
The assignment is divided into four main sections, demonstrating basic proficiency in navigating the Linux environment, monitoring system resources, managing background processes, checking network connectivity, and using Git for version control.

---

## 💻 Commands Executed

### Part 1: System Management
In this section, we checked the system's status and created the required directory and files to store the output.

* `whoami` : Displays the current logged-in username.
* `uname -a` : Displays detailed system and kernel information.
* `df -h` : Checks current disk space usage in a human-readable format.
* `free -m` : Displays current RAM/memory usage in megabytes.
* `mkdir linux_assignment` : Creates the new folder for the assignment.
* `cd linux_assignment` : Changes the directory into the newly created folder.
* `touch system.txt notes.txt` : Creates two empty text files.
* `uname -a > system.txt` : Writes the system information into the text file.
* `free -m >> system.txt` : Appends the memory usage information to the same text file without overwriting it.

### Part 2: Process Management
In this section, we monitored running tasks and practiced running and terminating processes in the background.

* `ps aux` : Lists all currently running processes on the system.
* `sleep 1000 &` : Starts a background process (sleeping for 1000 seconds). The `&` symbol forces it to the background.
* `jobs` : Displays the list of background jobs currently running in the terminal session.
* `kill %1` : Terminates the specified background job (in this case, job number 1).

### Part 3: Network Commands
In this section, we verified our internet connection and checked our local network settings.

* `ping -c 4 google.com` : Sends 4 network packets to Google's servers to verify internet connectivity.
* `ip a` : Displays the system's local IP address and network interface details.
* `ss -tuln` : Displays all open ports and listening sockets on the system.
* `ip a > network.txt` : Saves the IP address information into a new text file.

### Part 4: Git & GitHub
Finally, we initialized a local repository and pushed the created files to a remote GitHub repository.

* `git init` : Initializes a new, empty Git repository in the current folder.
* `git add .` : Stages all newly created text files for the first commit.
* `git commit -m "Complete Linux system management assignment"` : Commits the staged files with a descriptive message.
* `git branch -M main` : Renames the default branch to 'main'.
* `git remote add origin <repository-url>` : Links the local folder to the remote GitHub repository.
* `git push -u origin main` : Pushes the committed code up to GitHub using a Personal Access Token (PAT).
