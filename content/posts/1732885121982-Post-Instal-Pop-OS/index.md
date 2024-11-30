---
title: "Automating Post-Installation Setup on Pop!_OS with Custom Scripts"
date: 2023-11-22
draft: false
description: "a description"
tags: ["pop-os", "linux", "automation", "scripting", "development", "setup"]
---

Setting up a new operating system can be a tedious task, especially when it comes to installing essential software, configuring the environment, and setting up aliases for frequently used commands. To simplify this process, I created a set of scripts that automate the post-installation setup of Pop!_OS (22.04 LTS). In this post, we will take a look at the project and show how to use it to quickly set up your system.

{{< github repo="geraldohomero/post-install-pop-os" >}}

## Project Overview

The project consists of several scripts that perform various tasks, such as installing software packages, configuring custom aliases, and setting up the development environment. The main scripts are:

- [`run.sh`](run.sh): The entry point for the post-installation process.
- [`src/post-install.sh`](src/post-install.sh): Installs software packages and performs system cleanup.
- [`src/alias.sh`](src/alias.sh): Configures custom aliases.
- [`src/devEnv.sh`](src/devEnv.sh): Installs development tools like Node.js, .NET SDK, and Entity Framework Core.
- [`src/githubClone.sh`](src/githubClone.sh): Clones all repositories of a specified GitHub user.
- [`src/homeScript.sh`](src/homeScript.sh): Copies utility scripts to the home directory and makes them executable.
- [`misc/update.sh`](misc/update.sh): Updates and upgrades the system.
- [`misc/syncthingStatus.sh`](misc/syncthingStatus.sh): Checks the status of Syncthing.
- [`misc/swapAudio.sh`](misc/swapAudio.sh): Switches audio output channels.

```bash
LICENSE
misc/
  swapAudio.sh
  syncthingStatus.sh
  update.sh
README.md
run.sh
src/
  alias.sh
  devEnv.sh
  githubClone.sh
  homeScript.sh
  post-install.sh
```

## Getting Started

## Step 1: Clone the Repository

First, clone the repository to your preferred location. In this example, we will clone it to the `Downloads` folder:

```bash
git clone https://github.com/geraldohomero/post-install-pop-os.git $HOME/Downloads/post-install-pop-os
```

## Step 2: Make the Scripts Executable
Navigate to the cloned repository and make the scripts executable:
  
  ```bash
  cd $HOME/Downloads/post-install-pop-os
  chmod +x *.sh src/*.sh misc/*.sh
  ```
  

## Step 3: Run the Post-Installation Setup Script
Run the `run.sh` script to start the post-installation process:

The script will display colorful and informative messages as it progresses through the installation and configuration steps. You may need to provide your password for certain operations that require administrative privileges.

## Step 4: Follow the On-Screen Instructions
The setup script will guide you through the installation process. It will:

- Run the `src/post-install.sh` script to install software packages and perform system cleanup.
- Run the `src/alias.sh` script to configure custom aliases.
- Copy utility scripts (`update.sh`, `misc/syncthingStatus.sh`, and `misc/swapAudio.sh`) to the home directory and make them executable.
- Run the `src/devEnv.sh` script to install development tools.
- Run the `src/githubClone.sh` script to clone all repositories of a specified GitHub user.

## Step 5: Customize Aliases and Installed Programs
You can modify or add your own custom aliases in the `src/alias.sh` script to suit your workflow. Edit the `CUSTOM_ALIASES` array with the desired aliases and run the `src/alias.sh` script again to update your `.bash_aliases` file.

## Step 6: Review Installed Software and Aliases
After the setup is complete, you can review the installed software and aliases on your system. The `src/post-install.sh` script installs software packages listed in its configuration, while the `src/alias.sh` script configures custom aliases.

## Step 7: Use Utility Scripts
The utility scripts `misc/update.sh`, `misc/syncthingStatus.sh`, and `misc/swapAudio.sh` are copied to your home directory and made executable. You can use them as follows:

- `update`: Updates and upgrades the system.
- `syncstatus`: Checks the status of Syncthing.
- `swap`: Switches audio output channels.

## Conclusion
By following these steps, you can automate the post-installation setup for Pop!_OS, saving time and ensuring a consistent environment across installations. Feel free to customize the scripts to meet your specific needs and workflow.