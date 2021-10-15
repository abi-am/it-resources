## Unix users
Following command will create two files, your_key.rsa and your_key.rsa.pub.

`ssh-keygen -q -t rsa -f your_key.rsa -N ''`

Copy the content of your_key.rsa.pub file and send it to system administrator.

## Windows users
Use one of the provided methods to genrate key pair.

Method 1(not secure)
https://travistidwell.com/jsencrypt/demo/

Method 2
https://docs.joyent.com/public-cloud/getting-started/ssh-keys/generating-an-ssh-key-manually/manually-generating-your-ssh-key-in-windows

After generating the key, copy the public key content and send it to system administrator.
