# Windows-basic-commands-batchscript
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
![326683013-f1f83410-e659-40ff-bee3-e079d93c7736](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/7278ccac-404f-4fdb-b43d-e7f748c8fa69)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![326683213-4de1b4bd-f842-485a-bf0d-90def6eaf1e9](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/235bd8e6-5953-46be-a6d1-6fc8e2f925c7)

![326683200-60ef83ad-950a-4bf7-ae70-7ccd4fae7aa7](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/ab1a6add-1fab-47db-a752-7f6261c7d063)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![326683303-a28afee5-4fc8-4720-a29b-ae4c9819f177](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/7d444619-cd0a-417b-a7e6-5be47ce35a2e)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![326683342-ad0e4f9e-575b-48f5-95fe-7df3f52b5857](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/4d556f21-fb03-414c-95bc-4f92176f32b4)


![326683348-fc1a73ef-f263-4896-9465-239e1420b390](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/b9047423-b35f-4915-b24e-52617e83436e)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![326683386-0fe73689-4d9b-4494-8ce8-d940fc9b9606](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/40448f0c-6037-44e9-bc69-f1697ab0294f)

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


![326683409-f8257a6d-6fa4-4e1a-bc73-063fad3c5508](https://github.com/HARISHA2006/Windows-basic-commands-batchscript/assets/148843830/845add23-bd9b-4ece-978b-9b3059dade18)



# RESULT:
The commands/batch files are executed successfully.


