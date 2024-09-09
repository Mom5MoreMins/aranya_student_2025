---
layout: base
title: Journey
description: What Concepts I Learned and Used
hide: false
---
# Journey

## Setup

### Installing WSL and Setting up Ubuntu
1. To install Ubuntu 24.04 for WSL (Windows Subsystem for Linux):
   - Open PowerShell as an administrator and type:
     ```bash
     wsl --install -d Ubuntu-24.04
     ```
   - After the installation, set Ubuntu 24.04 as the default WSL distribution:
     ```bash
     wsl --set-default Ubuntu-24.04
     ```

### Cloning Repositories and Installing Necessary Tools
1. **Cloning the portfolio repository**:
   - In your home directory:
     ```bash
     cd
     mkdir nighthawk
     cd nighthawk
     git clone https://github.com/nighthawkcoders/portfolio_2025.git
     ```

2. **Running setup scripts**:
   - Navigate to the script directory and activate the Ubuntu setup script:
     ```bash
     cd nighthawk/portfolio_2025/scripts
     ./activate_ubuntu.sh
     ```

### Configuring GitHub Login
1. **Setting up GitHub credentials**:
   - Set your GitHub email:
     ```bash
     git config --global user.email "youremail@gmail.com"
     ```
   - Set your GitHub username:
     ```bash
     git config --global user.name "yourGHID"
     ```
   - Verify the configuration:
     ```bash
     git config --global --list
     ```

### Setting Up Your Project Repository
1. **Cloning the student project repository**:
   - In the `nighthawk` directory:
     ```bash
     git clone https://github.com/Mom5MoreMins/aranya_student_2025.git
     cd aranya_student_2025
     ```

2. **Preparing the project for development**:
   - Create and activate a virtual environment:
     ```bash
     scripts/venv.sh
     source venv/bin/activate
     ```
   - Install necessary Python packages:
     ```bash
     pip install -r requirements.txt
     ```
   - List installed Jupyter kernels to ensure Python3 is available:
     ```bash
     jupyter kernelspec list
     ```
   - Install necessary Ruby gems:
     ```bash
     bundle install
     ```
   - Open the project in VS Code:
     ```bash
     code .
     ```

3. **Local Server Setup**:
   - After configuring the `make` and `_config.yml` files, use the `make` command to run a local server:
     ```bash
     make 
     ```

---

## Important Commands

### Linux Command Line Basics
- `cd` - Change directories.
- `ls` - List files in the current directory.
- `chmod` - Change permissions on files. For example:
  ```bash
  chmod 755 filename
  ```

# Important Commands

## Linux Command Line Basics

- **`cd`**: This command allowed me to change directories. I used it frequently to move between folders on my system.
- **`ls`**: Using this, I could list the files and directories in my current directory, which helped me see what was inside each folder.
- **`chmod`**: I learned how to change file permissions using `chmod`. For example, the command `chmod 755 filename` gives:
  - `7 (rwx)`: Read, write, and execute permissions for the owner.
  - `5 (r-x)`: Read and execute permissions for the group.
  - `5 (r-x)`: Read and execute permissions for others.

## Bash Scripting and Editing Files

- I learned how to use Bash for running scripts, which allowed me to automate tasks.
- Used `vi` to edit configuration files directly from the command line. For example, running `vi filename` opened a file for editing.

## Git Commands

- **`git clone`**: This command allowed me to clone a repository from GitHub to my local machine.
- **`git add`**: Staged changes to be committed.
- **`git commit`**: Saved the staged changes with a descriptive message.
- **`git push`**: Pushed the committed changes to my remote repository on GitHub.

## Package Management with `apt` and `sudo`

- **`apt`**: Used for installing and managing software packages. For example, `apt install` allowed me to install necessary packages.
- **`sudo`**: Allowed me to run commands with administrative privileges, which was essential for making system-wide changes.

## Takeaways and Concepts Learned

Throughout this process, I learned how to effectively use the Linux command line for managing files, navigating directories, and setting permissions. I also became familiar with Git for version control, basic Bash scripting, and setting up and maintaining virtual environments for Python development.

Some struggles I encountered included understanding file permissions initially. The numeric system for setting permissions took some time to fully grasp. Additionally, I faced minor issues with missing dependencies when setting up the project environment, but I was able to troubleshoot those by reading error messages and installing the necessary packages.

Overall, this setup process provided me with a solid foundation in using command-line tools and version control, as well as in managing development environments.
