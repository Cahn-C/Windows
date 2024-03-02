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

<br>

## Variables

### Reading and defining variables

All variables in PowerShell start with a ```$``` followed by the name
```
$filePath
```

- Sometimes PowerShell does return an error if the variable isn't defined, so be sure to set a value in the variable

```
$filePath = 'C:\SomeFolder\Somewhere\file.txt'
```

Another way to set a variable, but in a more PowerShell way
```
Set-Variable -Name filePath -Value 'C:\SomeFolder\Somewhere\file.txt'
```

Get the value from the variable
```
Get-Variable -Name filePath
```

<br>

### Automatic Variables

Automatic variables read only varibales, meaning you can only get their values, you can't change them in any way

<br>

Get a list of all automatic variables
```
Get-Variable
```


This automatic variable defines how many lines of your command history are saved.
```
$MaximumHistoryCount
```

<br>

