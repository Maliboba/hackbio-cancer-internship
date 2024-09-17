# **Codes for Bash Project 1**

### Creating folders 
maliboba@DESKTOP-T336VHB:~$ `ls`

maliboba@DESKTOP-T336VHB:~$ `mkdir` `claudia`

maliboba@DESKTOP-T336VHB:$ `mkdir` `biocomputing`

maliboba@DESKTOP-T336VHB:$ `cd` `biocomputing`

## Dowloading files
maliboba@DESKTOP-T336VHB:~/biocomputing$ `wget` `https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna` `\`

wget ` https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk` `\`

wget `https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk` `\`

## Moving a file from folder biovcomputing to folder claudia
maliboba\@DESKTOP-T336VHB:\~/biocomputing$ `mv` `wildtype.fna` `~/claudia`

## Removing dupilcate of a file (wildtype.gbk)
maliboba@DESKTOP-T336VHB:~/biocomputing$ `rm` `-r` `wildtype.gbk.1`

## Finding wildtype and mutants
maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `"TATA"` `wildtype.gbk`

maliboba@DESKTOP-T336VHB:~/biocomputing$ ` grep` `"tatatata"` `wildtype.gbk`

## Printing mutant into a new file
maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `"tatatata"` `wildtype.gbk` `>` `mutant_lines.txt`&#x20;

## Viewing sequence
maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah yussif/Downloads$ `cat` `sequence.fasta`

## Moving fasta file from downloads to biocomputing
maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah yussif/Downloads$ `mv` `sequence.fasta`  `/home/maliboba/biocomputing`

## Changing directory to home
maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah yussif/Downloads$ `cd`

maliboba@DESKTOP-T336VHB:~$ `ls`

## Moving into biocomputing
maliboba@DESKTOP-T336VHB:$ `cd` `biocomputing`

## Listing contents 
maliboba@DESKTOP-T336VHB:~/biocomputing$ `ls`

## Renaming fasta
maliboba@DESKTOP-T336VHB:~/biocomputing$ `mv` `sequence.fasta` `BRCA1.fasta`

## Viewing sequences
maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `-v` `"^>"` `BRCA1.fasta` `|` `wc` `-l`

maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"A"` `|` `wc` `-l`

maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"G"` `|` `wc` `-l`

maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"C"` `|` `wc` `-l`

maliboba@DESKTOP-T336VHB:~/biocomputing$ `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"T"` `|` `wc` `-l`

## Creating a bash script
maliboba@DESKTOP-T336VHB:~/biocomputing$ `nano` `gc_content.sh`

## Making file executable 
maliboba@DESKTOP-T336VHB:~/biocomputing$ `chmod` `+x` `gc_content.sh`

## Running script
maliboba@DESKTOP-T336VHB:~/biocomputing$ `./gc_content.sh` `BRCA1.fasta`

maliboba@DESKTOP-T336VHB:~/biocomputing$ `nano` `Claudia.fasta`

## Viewing file
maliboba@DESKTOP-T336VHB:~/biocomputing$ `cat` `Claudia.fasta`

## Calling  A G T C in the file
maliboba@DESKTOP-T336VHB:~/biocomputing$ `echo` `"Number of A: $(grep -v "^>" Claudia.fasta | grep -o "A" | wc -l)"`

`echo` `"Number of G: $(grep -v "^>" Claudia.fasta | grep -o "G" | wc -l)"`

`echo` `"Number of T: $(grep -v "^>" Claudia.fasta | grep -o "T" | wc -l)"`

`echo` `"Number of C: $(grep -v "^>" Claudia.fasta | grep -o "C" | wc -l)"`
