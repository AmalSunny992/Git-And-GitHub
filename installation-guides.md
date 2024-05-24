# Installing Git on Windows

To install Git on Windows, follow these steps:

## Step 1: Download Git

1. Go to the [Git for Windows](https://gitforwindows.org/) website.
2. Click on the "Download" button to download the latest version of Git.

## Step 2: Install Git

1. Open the downloaded `.exe` file to start the installation process.
2. Follow the on-screen instructions:
   - **Select Destination Location**: Choose the default location or specify a different path.
   - **Select Components**: Select the components you want to install. The default selections are recommended.
   - **Adjusting Your PATH Environment**: Choose "Git from the command line and also from 3rd-party software".
   - **Choosing the SSH executable**: Use the OpenSSH included with Git.
   - **Choosing HTTPS transport backend**: Use the OpenSSL library.
   - **Configuring the line ending conversions**: Checkout Windows-style, commit Unix-style line endings.
   - **Configuring the terminal emulator**: Use MinTTY (the default terminal of MSYS2).
   - **Extra Options**: Enable file system caching and Git Credential Manager.
3. Click "Install" to complete the installation process.

## Step 3: Verify Installation

1. Open a command prompt (cmd) or Git Bash.
2. Type ``` git --version``` and press Enter. You should see the installed Git version.

You have successfully installed Git on Windows!


# Installing Git on MacOS

To install Git on macOS, follow these steps:

1. Go to the Git for macOS website.
2. Click on the "Download" button to download the latest version of Git.
3. Open the downloaded .dmg file and follow the on-screen instructions to install Git.

## Verify Installation on MacOs
1. Open the terminal.
2. Type ``` git --version ``` and press Enter. You should see the installed Git version.

You have successfully installed Git on macOS!

# Installing Git on Linux

To install Git on Linux, follow these steps based on your distribution:

## Debian/Ubuntu
1. Open the terminal.
2. Update the package list: sudo apt update
3. Install Git:
```sh
   sudo apt install git
```
## Fedora
1. Open the terminal.
2. Install Git:
```sh
   sudo dnf install git
```
## CentOS/RHEL
1. Open the terminal.
2. Install Git:
```sh
   sudo yum install git
```
## Arch Linux
1. Open the terminal.
2. Install Git:
```sh
   sudo pacman -S git
```
## Verify Installation on linux
Open the terminal.
Type ``` git --version ``` and press Enter. You should see the installed Git version.
