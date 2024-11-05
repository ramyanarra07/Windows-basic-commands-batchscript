# Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/b90b44da-d014-4e87-9497-70369505687e)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt
```


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/f8b14e97-065d-497c-86e9-30a0b5fa443e)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/2a57880c-f2ea-4286-9405-b22cb1b87ff5)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
move MyLab Documents
```
![image](https://github.com/user-attachments/assets/9aaeb38f-33e7-4a24-b226-dd4cb924045c)



## Exercise 2: Advanced Batch Scripting

Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup. If *.docx file are not available in the Documents folder you can use “.pdf” files to copy.

Open a notepad file named BackupScript.bat and enter the following:

## COMMAND
```
@echo off

mkdir %userprofile%\Desktop\DocBackup

copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup

echo Backup completed successfully!

```





## OUTPUT

![image](https://github.com/user-attachments/assets/8398cd51-0f5e-4544-aab3-ce1e91067bb4)




# RESULT:
The commands/batch files are executed successfully.

