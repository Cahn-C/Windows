## Running DOS Commands

### The following commands are considered as Aliases

Change directories
```
cd .\Windows\
```

List files and directories
```
dir
```

Clear the screen
```
cls
```

Execute ping.exe to ping an IP address
```
ping 1.1.1.1
```
```
ping www.example.com
```

<br>

## How Commands Work in PowerShell

Get a list of all commands in PowerShell
```
Get-Command
```

Get a list of all commands for a specifc verb
```
Get-Command -Verb Get
```
```
Get-Command -Verb Set
```
```
Get-Command -Verb New
```
```
Get-Command -Verb Add
```

Get al list of all services
```
Get-Service
```

<br>

## Getting Help

Understand the <i>Get-Help</i> command
```
Get-Help
```

Get the latest <i>Get-Help</i> features
```
Update-Help
```

Get information on a specific command
```
Get-Help -Name Get-Service
```
This is known as a positional parameter, meaning that you do not have to specify the <i>-Name</i> parameter
```
Get-Help Get-Service
```
