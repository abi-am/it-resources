# ABI IT resources: a user guide
Instructions for using computing resources at ABI

## Becoming a new user

### Step 1: generate a key pair

Follow [these instructions](https://github.com/abi-am/it-resources/blob/main/access-to-server/generating_key_pair.md) to generate a key pair. After you generate your key pair, keep the private key for yourself and give the public key to the server admin. He will create a user for you with a username of your choice.

### Step 2: access the server

Follow [these instructions](https://github.com/abi-am/it-resources/blob/main/access-to-server/) to access and login to the server. 

### Step 3: where to work

When you login to the server you will appear in the home directory. Don't do anything there. You need to redirect to the /storage/users/YOURUSERNAME or the /storage2/users/YOURUSERNAME directories and keep your private files there. Please, keep your workspace tidy. Remove the intermediate files as soon as possible so that there is space left for others to work. Note, that we are very limited in space right now. 

## Using the programs

Most of the programs you may need are installed on the server. [update from khach how to reveal the versions of installed software]. If a program is not installed, you should ask the team if it's of interest to others. If yes, ask the server admin to install it for all. If not, install it locally in your storage folder. 

## Running jobs
You can direclty run commands on the terminal only for a short period of time to test things. ATTENTION: DON'T RUN MEMORY-INTENSIVE JOBS from the terminal. After you've done testing the script, you should use SLURM resource distribution system to queue your job. Follow [these instructions](https://github.com/abi-am/it-resources/blob/main/using-the-server/slurm-instructions.md) for details.

## Shared project folders
Projects shared between multiple users can be deposited in the /storage and /storage2, in the folder named /proj. Use subfolders to specify your project. The name of the subfolder should adhere to the following format: PROJECTNAME_CORRESPONDINGUSER_YEAR. The project name should be as descriptive as possible. Each project should have a corresponding user responsible for its content, status, permissions, creation and deletion. You should also specify which year the project was built in. Each project folder should contain a README file where the description of the project, the list of all the users and their emails are posted. 

## Genome indices

The /storage/db folder contains genome builds and other common databases. If you need to use a genome indice you may specify the path to the corresponding files. DON'T COPY REFERENCE INDICES and DATABASES TO YOUR LOCAL FOLDERS. If you'd like to obtain a new genome index, you should build it locall adhering to the following [naming standards](https://github.com/abi-am/it-resources/blob/main/sop/genome_indices.md). After you're done with the build, send the path to your build to the server adiministrator to add it to the shared directory and remove it from your local directory. 

