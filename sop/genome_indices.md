The prebuilt genome indices should be stored in the /shared folder. 

## File tree
- organism-name
  - genome version
    - fa
    - gtf
    - gff
    - program
      - index files

Example file tree 

- homo-sapiens  
  - GRCh38.p13_GCA_000001405.28
    - fa
    - gtf
    - gff
    - star_1.2.8
      index files      
    - star_2.8.0
      index files
  - GRCh38.p14_GCA_000001805.02
    - fa
    - gtf
    - gff
    - bowtie_2.0.0    
      index files
- mus-musculus
  - ...


## Naming conventions

As shown in the file tree example above, each build folder should be named by the version of the genome, followed by an underscore, followed by the assembly accession. 
Inside the folder, there should always be subfolders named "fa", "gtf" or "gff" and "index" that contain the reference sequence FASTA file, the annotation files (optional) and the index files.

The programs used build the index should be named by the program name, followed by an underscore, followed by the program version. 

The organism names should be indicated with a dash. 
