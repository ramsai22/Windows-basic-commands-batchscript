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

### Developed by : paida ram sai
### Registered by : 212223110034




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![WhatsApp Image 2024-05-06 at 19 06 51_1dfd2d11](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/ad4c7446-2b1e-422b-b4bb-25a13353d62a)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![WhatsApp Image 2024-05-06 at 19 07 33_2761447e](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/3a6d27ff-deb5-4075-b57b-abffffb63379)
![WhatsApp Image 2024-05-06 at 19 07 47_e240f942](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/9a7000d9-41fd-4570-ad1a-d14678dd48d1)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![WhatsApp Image 2024-05-06 at 19 09 18_37e36bd9](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/9a8157df-3e61-473b-b60b-d6ebb3f56533)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup


copy MyFile.txt %userprofile%\Desktop\Backup

![WhatsApp Image 2024-05-06 at 19 09 57_58338354](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/461a975e-754f-4539-994d-428cdb869435)

![WhatsApp Image 2024-05-06 at 19 10 05_fe757bd6](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/448518a3-034d-42fa-8a0e-940a3fd0d434)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![WhatsApp Image 2024-05-06 at 19 10 49_9345172b](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/bef211d3-5a31-4651-a8c4-6032def7284a)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT
![WhatsApp Image 2024-05-06 at 19 11 56_76fbb043](https://github.com/23012653/Windows-basic-commands-batchscript/assets/150777517/47971ce1-a393-48ab-9f6a-7ebab394f1bb)







# RESULT:
The commands/batch files are executed successfully.

