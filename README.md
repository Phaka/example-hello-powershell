# Hello World in PowerShell

A minimal "Hello, World!" implementation in PowerShell. PowerShell is both a shell and a scripting language, originally developed by Microsoft for Windows system administration. It is now open-source and cross-platform through PowerShell Core.

## Installation

### Windows
PowerShell comes pre-installed on modern Windows systems. PowerShell Core can be installed from the Microsoft Store or downloaded from GitHub.

### macOS
Using Homebrew:
```bash
brew install powershell
```

### Linux
Ubuntu/Debian:
```bash
# Download the Microsoft repository GPG keys
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb
# Register the Microsoft repository GPG keys
sudo dpkg -i packages-microsoft-prod.deb
# Update package list
sudo apt-get update
# Install PowerShell
sudo apt-get install -y powershell
```

For other distributions, see the [PowerShell documentation](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell).

## Running

Execute the script directly:
```powershell
pwsh ./main.ps1
```

Or on Windows, you can also use:
```powershell
powershell.exe -File main.ps1
```

## Code Explanation

The program uses `Write-Output`, which is a PowerShell cmdlet (command-let) that writes objects to the pipeline. While this simple example might look similar to other languages' print statements, PowerShell's `Write-Output` can handle complex .NET objects, not just strings. This reflects PowerShell's object-oriented approach to shell scripting, where commands pass entire objects through pipelines rather than just text streams.
