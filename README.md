# Remote Code Execution Exploit Script

This Bash script automates the process of exploiting a vulnerable web application to achieve remote code execution (RCE) by uploading a malicious PHP script. The script performs the following key functions:

Features

1. Login to the Web Application: The script first logs into the target web application using predefined credentials to establish a session.

2. Create Malicious PHP Script: It generates a PHP script (root.php) that executes system commands passed via a GET parameter.

3. Upload the Malicious Script: The script uploads the generated PHP script alongside other necessary dummy files to the target web application.

4. Command Execution Loop: After uploading the malicious script, the user is prompted to enter system commands to execute on the server. The output of the commands is retrieved and displayed.

5. Cleanup: After the user exits the command loop, the script removes the uploaded files and temporary cookie files used for the session.

Usage

To use this script, run it from the command line with the target IP address and port number as arguments:

```bash
./exploit.sh <IP_ADDRESS> <PORT>


REF : https://github.com/HKD01l/bug_report/blob/main/vendors/mayuri_k%20canteen-management-system/RCE-1.md
