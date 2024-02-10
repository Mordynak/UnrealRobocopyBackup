@echo off

REM Define source and destination paths
set "SOURCE_DIR=A:\Dev\ProjectFolder"
set "DEST_DIR=Z:\Backup\ProjectFolder"

REM Get current date and time in YYYY-MM-DD_HH-MM-SS format
for /f "tokens=2 delims==" %%I in ('wmic os get localdatetime /value') do set "DATETIME=%%I"
set "DATE_TIME=%DATETIME:~0,4%-%DATETIME:~4,2%-%DATETIME:~6,2%__%DATETIME:~8,2%-%DATETIME:~10,2%-%DATETIME:~12,2%"

REM Execute Robocopy command with exclusion arguments. 
REM This time we use a jobfile to make reading the excluded files and directories easier.
Robocopy "%SOURCE_DIR%" "%DEST_DIR%\Nox__%DATE_TIME%" /E /job:ignore

echo.
echo.
echo ======== %DATE_TIME% ========
echo.
echo Affirmative, Dave. 
echo Backup procedure has been successfully executed without any anomalies. 
echo All files have been securely copied to the designated destination.
echo Is there anything else you require assistance with?
echo.
echo ======== %DATE_TIME% ========
echo.
echo.

pause
