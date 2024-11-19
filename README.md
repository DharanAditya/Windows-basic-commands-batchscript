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

Developed by: DHARAN ADITYA

Register number: 212223040035

## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/971cebbc-c9d2-44fc-adc9-2b1152a6c55e)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/2af10eb7-2f56-446c-a992-c64acc38ebd7)

```
type nul > MyFile.txt
```

![image](https://github.com/user-attachments/assets/e19ec36d-fa54-4a5e-bd30-183ae6179a20)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/29fc03f5-5523-4eb2-a39c-f2e01c38a879)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```

![Screenshot 2024-11-18 222823](https://github.com/user-attachments/assets/8a1cc2e2-cf19-4c12-ba57-a22dc159a350)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/befc4d9c-847c-4fc8-b89d-3ba21a5646ba)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![image](https://github.com/user-attachments/assets/7f547ed6-f06f-4794-8335-21202d139d39)


## Exercise 2: Advanced Batch Scripting

Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT

![image](https://github.com/user-attachments/assets/07d0b6b5-0395-49b8-82a2-f0c5633baadf)


## COMMAND:

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

![image](https://github.com/user-attachments/assets/09b9b2b4-239f-4bb4-8269-f6f34e0a8a12)


# RESULT:
The commands/batch files are executed successfully.

