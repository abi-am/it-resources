
1. Open the command line by keyboard shortcut Ctrl-Alt+T

2. Move the provided key file to the .ssh directory:

`mv your_key ~/.ssh`

If the key is not provided than you should provide your public key to system administrator. 
If you don't have a pablic/private key, create one with this command:

`ssh-keygen -q -t rsa -f your_key.rsa -N ''`

This command will create two files, _your_key.rsa_ and _your_key.rsa.pub_. Copy the content of _your_key.rsa.pub_ file and send it to system administrator.
Then move created key file to the .ssh directory:

`mv your_key ~/.ssh`

3. Change the permissions of the key file so only the root user can read it:

`chmod 400 ~/.ssh/your_key.rsa`

4. Connect to server via this command:

`ssh -i ~/.ssh/your_key.rsa username@server_ip`
