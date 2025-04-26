# probable-chainsaw
Passion for technology preferably on WSL

# Enabling WSL on your Windows System, specifically WSL2

Make sure the box is checked.
1. Windows Subsystem for Linux
2. Virtual Machine Platform
   
![windows_features](https://github.com/user-attachments/assets/d8a4f8da-4eeb-453d-a93c-bc903662688b)

Restart the system

# Installing a Linux distribution


![username](https://github.com/user-attachments/assets/a3b679f5-c66b-4353-bb59-2dd89659d78f)

# Using Windows cmd.exe

run prompt | `"windows" key + r`

Open: `cmd`



```python
# First update the Windows Subsystem for Linux package.
>wsl --update

# Check to see the state of your instance (RUNNING | STOPPED)
>wsl --list --verbose

>wsl --status
```



# Using the wsl.exe tool

wsl.exe from Windows cmd.exe will open on `/mnt/c` Windows file system.
You want it to open in your Linux home directory. It is important to understand when you work inside `/mnt/c` you're interacting with Windows files.

`wsl.exe ~`


![wsl](https://github.com/user-attachments/assets/a4527805-ed7e-4caf-ba02-8e9f772311ed)






