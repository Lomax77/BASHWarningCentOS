# BASHWarningCentOS
Pop-up notification for CentOS/Redhat 7
Make sure Notify is installed

**#sudo yum install libnotify**

Save the script into a file (for example warning.sh) and make the script executable with chmod +x warning.sh.

You can then run this script in the background using:

**#nohup ./warning.sh &**

The nohup command makes sure the script continues running even if you close the terminal. & makes it run in the background.

If you want to stop the script, you'll need to find its process ID (PID) and kill it. You can find the PID using the ps command and looking for your script's name, then kill it with the kill command.

**ps aux | grep warning.sh**

**kill -9 PID**

Replace PID with the actual process id number from the output of the ps command.
