# Window-Server-backup

In Windows Server Backup, when restoring data to a user's system, the backup process often saves the data in ISO format. However, instead of converting the backup to an ISO file, it is possible to retain the original file format. To achieve this, we can write a batch file.

The `@echo off` command in the batch file ensures a cleaner output by suppressing the display of commands during execution. The `Robocopy` command, a robust file-copying tool in Windows, can efficiently copy files, directories, and entire folder trees while handling errors and maintaining file attributes. For example, the command `Robocopy "C:\new folder" "D:\backup_folder"` copies all files from the source directory (`C:\new folder`) to the destination directory (`D:\backup_folder`). Adding options like `/E` ensures that all subdirectories are included, even if they are empty. The `pause` command can be added to halt the script after execution, allowing the user to review the output.
