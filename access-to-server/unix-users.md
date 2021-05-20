
1. Open the command line by keyboard shortcut Ctrl-Alt+T

2. Move the downloaded key file to the .ssh directory:

`mv your_key ~/.ssh`

3. Change the permissions of the key file so only the root user can read it:

`chmod 400 ~/.ssh/your_key`

4. Connect to server via this command:

`ssh -i ~/.ssh/your_key username@185.127.66.93`
