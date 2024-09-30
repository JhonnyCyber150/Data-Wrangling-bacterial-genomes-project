# Data Wrangling - Bacterial-genomes-project


To downloads the file go to the website https://www.ncbi.nlm.nih.gov/datasets/ 

### Follow the steps

1. Select genomes 
2. Click bacteria and there are about 2.1 millions 
3. Click total
4. Set columns and choose (GC percentage, Contig N50,
5. Scaffold count, genome size)
6. Sort the date and select the 14 genomes release up to 2001
7. Download
#### downlad package (~18 mb)

## Create a README.md file
Go to link https://github.com/ and create an acount  and an repository 

# Question 2
## Copy the files to your home directory on IBEX and uncompress

### To copy to my home directory 

``` bash 
scp C:\Users\USUARIO\Downloads\bacterial_dataset.zip caichoj@ilogin.ibex.kaust.edu.sa:~/  
```
Enter the password 

The file has been copied

``` bash 
bacterial_dataset.zip                                                                 100%   16MB   5.1MB/s   00:03
```

To verify the upload to the ibex
```bash 
after put ls -l
total 26320
-rw-r--r--  1 caichoj g-caichoj 16768029 Sep 23 03:14 bacterial_dataset.zip
-rw-r--r--  1 caichoj g-caichoj      111 Sep 22 12:10 cpu_ibex.slurm
-rw-r--r--  1 caichoj g-caichoj     1041 Sep 17 17:15 E_coli_first10.fna
-rw-r--r--  1 caichoj g-caichoj  5018316 Sep 22 16:07 ecoli.fna
-rw-r--r--  1 caichoj g-caichoj  5018316 Sep 17 15:03 Ecoli.fna
drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:12 genomes
-rw-r--r--  1 caichoj g-caichoj      229 Sep 22 12:26 gpu_ibex.slurm
drwxr-xr-x 30 caichoj g-caichoj     4096 Sep 17 16:50 ncbi.dataset.tsv
drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:33 new_genomes
```
Notice bacterial_dataset.zip has been added 

### To unzip
```bash 
[caichoj@login509-02-r ~]$ unzip bacterial_dataset.zip
```

During the unzip

```bash 


Archive:  bacterial_dataset.zip
  inflating: README.md
  inflating: ncbi_dataset/data/data_summary.tsv
  inflating: ncbi_dataset/data/assembly_data_report.jsonl
  inflating: ncbi_dataset/data/GCA_000008525.1/GCA_000008525.1_ASM852v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008605.1/GCA_000008605.1_ASM860v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008625.1/GCA_000008625.1_ASM862v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008745.1/GCA_000008745.1_ASM874v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000027305.1/GCA_000027305.1_ASM2730v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008525.1/GCF_000008525.1_ASM852v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008605.1/GCF_000008605.1_ASM860v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008625.1/GCF_000008625.1_ASM862v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008745.1/GCF_000008745.1_ASM874v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000027305.1/GCF_000027305.1_ASM2730v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000006745.1/GCA_000006745.1_ASM674v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008545.1/GCA_000008545.1_ASM854v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008565.1/GCA_000008565.1_ASM856v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008725.1/GCA_000008725.1_ASM872v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000008785.1/GCA_000008785.1_ASM878v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000006745.1/GCF_000006745.1_ASM674v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008545.1/GCF_000008545.1_ASM854v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008565.1/GCF_000008565.1_ASM856v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008725.1/GCF_000008725.1_ASM872v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000008785.1/GCF_000008785.1_ASM878v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000006825.1/GCA_000006825.1_ASM682v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000006865.1/GCA_000006865.1_ASM686v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000007125.1/GCA_000007125.1_ASM712v1_genomic.fna
  inflating: ncbi_dataset/data/GCA_000091085.2/GCA_000091085.2_ASM9108v2_genomic.fna
  inflating: ncbi_dataset/data/GCF_000006825.1/GCF_000006825.1_ASM682v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000006865.1/GCF_000006865.1_ASM686v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000007125.1/GCF_000007125.1_ASM712v1_genomic.fna
  inflating: ncbi_dataset/data/GCF_000091085.2/GCF_000091085.2_ASM9108v2_genomic.fna
  inflating: ncbi_dataset/data/dataset_catalog.json
  inflating: md5sum.txt

```

ls -l

appear new files in my home directory like ncbi_dataset and README.md, md5sum.text

```bash 
rw-r--r--  1 caichoj g-caichoj 16768029 Sep 23 03:14 bacterial_dataset.zip
-rw-r--r--  1 caichoj g-caichoj      111 Sep 22 12:10 cpu_ibex.slurm
-rw-r--r--  1 caichoj g-caichoj     1041 Sep 17 17:15 E_coli_first10.fna
-rw-r--r--  1 caichoj g-caichoj  5018316 Sep 22 16:07 ecoli.fna
-rw-r--r--  1 caichoj g-caichoj  5018316 Sep 17 15:03 Ecoli.fna
drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:12 genomes
-rw-r--r--  1 caichoj g-caichoj      229 Sep 22 12:26 gpu_ibex.slurm
-rw-------  1 caichoj g-caichoj     3165 Sep 22 19:22 md5sum.txt
drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 23 03:21 ncbi_dataset
drwxr-xr-x 30 caichoj g-caichoj     4096 Sep 17 16:50 ncbi.dataset.tsv
drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:33 new_genomes
-rw-------  1 caichoj g-caichoj     1593 Sep 22 19:22 README.md
```


# Questions 3
### What is the smallest and what is the largest genome

Command 
``` bash
find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -exec sh -c 'echo "$(tail -n +2 "$1" | wc -c) $(basename "$1")"' _ {} \; | sort -n | tail -n 1 | awk '{print "Largest genome is in file \"" $2 "\": " $1}'
```

Output:

# Questions 4
### Find the number of genomes that contain at least two “c”

Output:


# Question 5 
### Use find command to find all genome files (FASTA) largerthan 3 megabyte.

Output:
