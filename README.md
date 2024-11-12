NAME: VARSHA SARATHY
REG NO:212223040233

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


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/a7c9a6e8-1fca-4f10-b778-15ec14db970e)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/dc8f9df1-5957-4ca5-9ad3-0eaca38b92cf)

```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/8de559b7-6ec6-4443-ab2a-1089e35bdeb5)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/9c86a7d9-1950-42fc-8f96-108202c2207c)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/1b989ee9-2710-4302-925c-05b82f0b0d16)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/32b0be5f-6a2b-4bc6-bc27-a6a521cbe909)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/c6ed7b05-db8f-4e12-aa33-50fa0ab8fe82)

## Exercise 2: Advanced Batch Scripting

Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![image](https://github.com/user-attachments/assets/be369451-cd4b-4f84-94e9-4e19605a3a6c)

COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/295627eb-a969-4ff4-a2f5-4cc6bd5cdf06)

# RESULT:
The commands/batch files are executed successfully.

