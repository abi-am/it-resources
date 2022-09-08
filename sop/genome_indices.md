The prebuilt genome indices should be stored in the /shared folder. 

## File tree
- organism-name
  - program
    - genome version
      - index files

Example file tree 

- homo-sapiens
  - star_1.2.8
    - GRCh38.p13_GCA_000001405.28
      - fa
      - gtf
      - gff
      - index
        - index files
    - GRCh38.p10_GCA_000001305.21
  - star_2.8.0
    - GRCh38.p13_GCA_000001405.28
  - bowtie_2.0.0
    - GRCh38.p13_GCA_000001405.28
- mus-musculus
  - ...


## Naming conventions

As shown in the file tree example above, each build folder should be named by the version of the genome, followed by an underscore, followed by the assembly accession. 
Inside the folder, there should always be subfolders named "fa", "gtf" or "gff" and "index" that contain the reference sequence FASTA file, the annotation files (optional) and the index files.

The programs used build the index should be named by the program name, followed by an underscore, followed by the program version. 

The organism names should be indicated with a dash. 
