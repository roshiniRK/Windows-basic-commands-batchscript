# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

Developed By: ROSHINI R K

Reg No: 212222230123

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

mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/5b9e9b36-ef0a-4ee7-a855-8703f462fdc9)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/9a9c8ae2-ee6d-4dbc-9632-4b1a8f7f7919)

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/e178db40-9af0-45aa-ac74-1fc6dd75601d)



List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/18115e64-3f55-4b04-825e-5ed79b0a3815)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/ff672c06-cc47-49d9-9a8c-d321b732090f)

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/bc7cda54-748e-42d6-8cc6-15afbdcd1dc7)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/59a14bc4-3c4f-42ec-b639-7807bd71d955)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![image](https://github.com/roshiniRK/Windows-basic-commands-batchscript/assets/118956165/e0e73bb5-2c70-4c64-b077-d6abc0a8f318)


# RESULT:
The commands/batch files are executed successfully.

