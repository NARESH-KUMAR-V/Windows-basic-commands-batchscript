# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![ex8op1](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/2aeb7c7e-b773-48d4-8e25-c07a11216a1a)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```
![ex8op2](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/e9e61dc2-f6a6-4ff8-9c29-09ce1ce5c8f5)


```
type nul > MyFile.txt
```
![ex8op3](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/873a293d-cea0-4ca5-bd63-acca1909b7b9)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![ex8op4](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/010d2c2b-6407-47ff-91b9-8d3c7fa5125f)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
```
![ex8op5](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/d8d98071-8756-4605-8712-730e5018761c)


```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![ex8op6](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/10f1fbc6-bce9-4678-82a9-d2ccb9ce82ff)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![ex8op7](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/519a76b8-280d-4d1b-a925-d3cf35305261)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


## OUTPUT:
![ex8op8](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/cb129b0f-c797-4fc7-b4d3-4b8435ab31af)


## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:
![ex8op9](https://github.com/NARESH-KUMAR-V/Windows-basic-commands-batchscript/assets/145842937/c6d005ab-f5b7-403b-8bfe-ae1cd1df179e)

# RESULT:
The commands/batch files are executed successfully.

