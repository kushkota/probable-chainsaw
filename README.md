# probable-chainsaw
Passion for technology preferably on WSL

## Enabling WSL on your Windows System, specifically WSL2

Make sure the box is checked.
1. Windows Subsystem for Linux
2. Virtual Machine Platform
   
![windows_features](https://github.com/user-attachments/assets/d8a4f8da-4eeb-453d-a93c-bc903662688b)

Restart the system

## Installing a Linux distribution


![username](https://github.com/user-attachments/assets/a3b679f5-c66b-4353-bb59-2dd89659d78f)

## Using Windows cmd.exe

run prompt | `"windows" key + r`

Open: `cmd`



```python
# First update the Windows Subsystem for Linux package.
>wsl --update

# Check to see the state of your instance (RUNNING | STOPPED)
>wsl --list --verbose

>wsl --status
```



## Using the wsl.exe tool

wsl.exe from Windows cmd.exe will open on `/mnt/c` Windows file system.
You want it to open in your Linux home directory. It is important to understand when you work inside `/mnt/c` you're interacting with Windows files.

`wsl.exe ~`


![wsl](https://github.com/user-attachments/assets/a4527805-ed7e-4caf-ba02-8e9f772311ed)

# Distribution configuration with wsl.config



Customize the Linux system's host name within WSL rather than using the defaults, which is the Windows PC name.

1. Edit Configuration File:
   - `sudo vim /etc/wsl.config`
   - Add highlighted entry on the config file
  
![hostname](https://github.com/user-attachments/assets/11f575ca-0bf0-40e2-9cee-6aa603b262ca)


3. Start fresh:
   - Shut it down manually ( `wsl --shutdown` ) or,
   - Wait for the system's virtual machine (VM) to automatically shutdown ( when no processes are running)

Results:

* Inside your Linux environment: The host name will appear as `myWSL

* From the perspective of the Windows host, the Linux environment in WSL is still accessed using `localhost`, which is the default network lookback address (127.0.0.1).

## Using GUI apps invoking via WSL2 

This change version control is coming from VS code Mac


```python

# adding a comment here from Windows path of executable
learnwsl@myWSL:~$ /mnt/c/Program\ Files\ \(x86\)/Google/Chrome/Application/chrome.exe
```








