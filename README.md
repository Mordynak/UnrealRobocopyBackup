# Unreal Engine Project Robocopy Incremental Backup
Simple script with the intention of creating an incremental timestamped backup of Unreal Project and Source Art folders.

## Usage
Two variants of the backup script to use. 
"backupUE.bat" is a self contained script which contains all the exclusions.
"BackupUE_IgnoreJob.bat" uses an external ignore file (ignore.rcj) to manage the excluded files and directories. Easier for editing and readability. Both files are required.

Simply alter the source and destination directory of either method you choose to your liking and double click the .bat file to run.
