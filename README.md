# bacterial-genomes-project

To downloads the file go to the website (https://www.ncbi.nlm.nih.gov/datasets/)
Follow the steps

selecionamos genomes
click bacteria y sale com 2.1 millions
click en total 
luego set columns y colocamos las 4 opciones
luego invertimos el date (click sobre release) y seleccionamos los 14 que son up 2001

en downland selecciona el dowland package (peas 18 mb)

# Question 2
scp C:\Users\USUARIO\Downloads\bacterial_dataset.zip caichoj@ilogin.ibex.kaust.edu.sa:~/  

I should enter the passowrd and it was copied

SMS output 
bacterial_dataset.zip                                                                 100%   16MB   5.1MB/s   00:03


To verify the upload to the ibex: ls -l

  ##total 26320
  
  -rw-r--r--  1 caichoj g-caichoj 16768029 Sep 23 03:14 bacterial_dataset.zip   
  -rw-r--r--  1 caichoj g-caichoj      111 Sep 22 12:10 cpu_ibex.slurm   
  -rw-r--r--  1 caichoj g-caichoj     1041 Sep 17 17:15 E_coli_first10.fna  
  -rw-r--r--  1 caichoj g-caichoj  5018316 Sep 22 16:07 ecoli.fna  
  -rw-r--r--  1 caichoj g-caichoj  5018316 Sep 17 15:03 Ecoli.fna  
  drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:12 genomes  
  -rw-r--r--  1 caichoj g-caichoj      229 Sep 22 12:26 gpu_ibex.slurm  
  drwxr-xr-x 30 caichoj g-caichoj     4096 Sep 17 16:50 ncbi.dataset.tsv  
  drwxr-xr-x  3 caichoj g-caichoj     4096 Sep 22 15:33 new_genomes  

  It seems that the file.zip has been uploaded
  
##To unzip: unzip bacterial_dataset.zip

  Output 

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

  TO verify the unzip files in the home directory: ls -l

  appear new files in my home directory like ncbi_dataset and README.md, md5sum.text

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


# Questions 3 Largest and Smallest file 
  Largest genome
  
  Code:
  
  find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -exec sh -c 'echo "$(tail -n +2 "$1" | wc -c) $(basename "$1")"' _    {} \; | sort -n | tail -n 1 | awk '{print "Largest genome is in file \"" $2 "\": " $1}'

  Output:
  
  Largest genome is in file "GCF_000006745.1_ASM674v1_genomic.fna": 4083974

  Smallest genome
  
  Code:
  
  Find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -exec sh -c 'echo "$(tail -n +2 "$1" | wc -c) $(basename "$1")"' _     {} \; | sort -n | head -n 1 | awk '{print "Smallest genome is in \"" $2 "\": " $1}'

  output: 
  
  Smallest genome is in "GCA_000008725.1_ASM872v1_genomic.fna": 1055551 
  
  
  
  # Questions 4 Genomes that contain at least two "C" 

  the first part for files that contain at least two "C"
  
  code:
  
  find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -exec sh -c 'grep -E "^>" "$1" | awk -F " " "{print \$2}" | grep -E   "c.*c" | wc -l' _ {} \; | awk '{total += $1} END {print total}'
  
  output:
  
  14

  the second part that doesnt have "coccus" 

  Code:
  
  find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -exec sh -c 'grep -E "^>" "$1" | awk -F " " "{print \$2}" | grep -E   "c.*c" | grep -v "coccus" | wc -l' _ {} \; | awk '{total += $1} END {print total}'

  output:
  
  4



  # Q5 files lager than +3M
  
  Code:
  
  find /home/caichoj/ncbi_dataset/data -type f -name "*.fna" -size +3M | wc -l

  Output:
  
  6
