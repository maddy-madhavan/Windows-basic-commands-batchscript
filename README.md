# Windows-basic-commands-batchscript
# Name:madhavan k
# Reg No: 212224220054

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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-13 111833](https://github.com/user-attachments/assets/b1a58131-f1d3-454b-bb8e-f43e323c546d)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-13 111923](https://github.com/user-attachments/assets/59237b43-5e97-43ce-8fbc-ea58e0c4591e)

![Screenshot 2025-05-13 111929](https://github.com/user-attachments/assets/89d66e98-4131-443e-a093-4407cd8a0a58)




## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-13 112013](https://github.com/user-attachments/assets/20d7c37d-8475-4ffc-9f49-75f73f0ec603)



## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-13 112115](https://github.com/user-attachments/assets/671edcc0-d33d-43d4-b071-79cf6990f2d3)

![Screenshot 2025-05-13 112123](https://github.com/user-attachments/assets/6447142c-180d-445f-ae8e-f03326999700)





## COMMAND AND OUTPUT


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
![Screenshot 2025-05-13 112317](https://github.com/user-attachments/assets/5676f936-2376-425c-a07a-fac1134f98ff)





# RESULT:
The commands/batch files are executed successfully.
