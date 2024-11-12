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
![image](https://github.com/user-attachments/assets/db176217-6b0a-4119-adcc-037e0d7468fa)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/74056cbd-6c6b-4e87-a57e-66ac74811d71)

```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/a257d226-7872-4d45-aee0-243c26b3339b)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/a5013fba-5597-4f4c-8f24-05427169582d)

```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/ff57fa1d-ad78-4587-9287-98245a788d92)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/77578822-90c0-4314-a3ee-0ecead765459)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/2341807f-37a2-493f-b920-10525e6a0d43)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![image](https://github.com/user-attachments/assets/085031d4-c75b-4925-b69f-03ac94182337)

COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/c7cde5cb-73a3-418a-b503-56560ca3f364)

# RESULT:
The commands/batch files are executed successfully.
