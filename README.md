# ABI IT resources

Instructions for using computing resources at ABI

## Becoming a new user

### Step 1: generate a key pair and access the server

Follow [these instructions](/access-to-server/howto.md) to generate a key pair. After you generate your key pair, keep the private key for yourself and give the public key to the server admin. He will create a user for you and report back your username.

Go back to the instructions to learn more about accessing the server.

### Step 2: where to work

When you login to the server you will appear in the home directory. Don't do anything there. You need to redirect to the /storage/users/YOURUSERNAME or the /storage2/users/YOURUSERNAME directories and keep your private files there. Please, keep your workspace tidy. Remove the intermediate files as soon as possible so that there is space left for others to work. Note, that we are very limited in space right now. Before running any storage intensive job or downloading big data files ALWAYS check available storage with the following command:
``df -h .``

## Using the programs

Most of the programs you may need are installed on the server. [update from khach how to reveal the versions of installed software]. If a program is not installed, you should ask the team if it's of interest to others. If yes, ask the server admin to install it for all. If not, install it locally in your storage folder. 

## Running jobs

You can direclty run commands on the terminal only for a short period of time to test things. ATTENTION: DON'T RUN MEMORY-INTENSIVE JOBS from the terminal. After you've done testing the script, you should use SLURM resource distribution system to queue your job. Follow [these instructions](https://github.com/abi-am/it-resources/blob/main/using-the-server/slurm-instructions.md) for details.
