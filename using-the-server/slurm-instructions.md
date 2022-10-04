# Using SLURM to run jobs

1. Create an example script named slurm_example.sh:

```
#!/bin/bash  				
#SBATCH --mem 10gb			# the amount of memory you request for your job
#SBATCH --cpus-per-task=4           # Number of CPU cores per task
#SBATCH --output=slurm-%j.log		# file name where the job console output will be stored
#SBATCH --mail-type=BEGIN,END		# if specified you will receive email when your job starts, ends	
#SBATCH --mail-user=<your_mail>		# your email address

for i in {1..100..1}				your script
do
    echo "This is my first script with slurm :)"
done

```

2. Submit the job script:

```
sbatch slurm_example.sh
```

3. Check the job status:

```
squeue 
```

4. Cancel your pending or running job:

```
scancel 3564
```


For more detailed information see the [slurm documentation](https://slurm.schedmd.com/documentation.html).
