# CITN PowerShell

Welcome Church IT Network folks!

Below you should find some links to get you started with Powershell.

# 3 Things you should should know!

### 1. If you only use Get commands you can't do any damage!

You can use Get-Command to see what commands you can get.

`Get-Command get-*`

`Get-Command get-* -Module ActiveDirectory`

`Get-Help`

If you get an error when you try to get help then you should update help and this is the way to do it:

`Update-Help`

### 2. You can count Objects

The command below will get all the Processes on your computer.

`Get-Process`

But if you want to count the Processes you simply surround it with Parentheses like this and view the count.

`(Get-Process).count`

### 3. You can grab powershell on another computer

There are some tricks to getting remote powershell to work right - this isn't a tutorial on Remoting... but if you have fairly new OSs on machines,
you can connect to another Machine using the Enter-PSsession command:

`Enter-PSSession DC1`


## Learning Powershell 

- [Best Tutorial](https://channel9.msdn.com/Series/GetStartedPowerShell3/01)



### PowerShell Editor


I prefer to  use Visual Studio Code (VS Code) which works on Windows, Linux, and macOS.
Click on the following link to create your first PowerShell script.

- [Using Visual Studio Code (VS Code)](https://docs.microsoft.com/powershell/scripting/dev-cross-plat/vscode/using-vscode)


## Installing PowerShell

First you need to set up your computer working environment if you have not done so.
Choose the platform below and follow the instructions.
At the end of this exercise, you should be able to launch the PowerShell session.

- Get PowerShell by installing package
    * [PowerShell on Windows][inst-win]
    * [PowerShell on macOS][inst-macos]
    * [PowerShell on Linux][inst-linux]


  For this tutorial, you do not need to install PowerShell if you are running on Windows.
  You can launch PowerShell console by pressing Windows key, typing PowerShell, and clicking on Windows PowerShell.
  However if you want to try out the latest PowerShell, follow the [PowerShell on Windows][inst-win].

- Or you can get the PowerShell by [building it][build-powershell]

[build-powershell]:../../README.md#building-the-repository
[inst-linux]: https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-linux
[inst-win]: https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows
[inst-macos]: https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-macos
