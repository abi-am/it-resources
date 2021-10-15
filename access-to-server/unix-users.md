
1. Open the command line by keyboard shortcut Ctrl-Alt+T

2. Move the key file to the .ssh directory:

`mv your_key ~/.ssh`

3. Change the permissions of the key file so only the root user can read it:

`chmod 400 ~/.ssh/your_key.rsa`

4. Connect to server via this command:

`ssh -i ~/.ssh/your_key.rsa username@server_ip`
