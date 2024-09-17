`maliboba@DESKTOP-T336VHB:~$` `ls`

`maliboba@DESKTOP-T336VHB:~$` $ `mkdir` `stage1_assign`

`maliboba@DESKTOP-T336VHB:$` `mkdir` `biocomputing`

`maliboba@DESKTOP-T336VHB:$` `cd` `biocomputing`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `wget` `https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna` `\`

wget ` https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk` `\`

wget `https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk` `\`

maliboba\@DESKTOP-T336VHB:\~/biocomputing$ `mv` `wildtype.fna` `~/stage1_assign`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `rm` `-r` `wildtype.gbk.1`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `"TATA"` `wildtype.gbk`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` ` grep` `"tatatata"` `wildtype.gbk`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` $ `grep` `"tatatata"` `wildtype.gbk` `>` `mutant_lines.txt`&#x20;

`maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah` `yussif/Downloads`$ `cat` `sequence.fasta`

`maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah` `yussif/Downloads`$ `mv` `sequence.fasta`  `/home/maliboba/biocomputing`

`maliboba@DESKTOP-T336VHB:/mnt/c/Users/musah` `yussif/Downloads`$ `cd`

`maliboba@DESKTOP-T336VHB:~$` `ls`

`maliboba@DESKTOP-T336VHB:$` `cd` `biocomputing`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `ls`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `mv` `sequence.fasta` `BRCA1.fasta`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `-v` `"^>"` `BRCA1.fasta` `|` `wc` `-l`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"A"` `|` `wc` `-l`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"G"` `|` `wc` `-l`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"C"` `|` `wc` `-l`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `grep` `-v` `"^>"` `BRCA1.fasta` `|` `grep` `-o` `"T"` `|` `wc` `-l`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `nano` `gc_content.sh`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `chmod` `+x` `gc_content.sh`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `./gc_content.sh` `BRCA1.fasta`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `nano` `Claudia.fasta`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `cat` `Claudia.fasta`

`maliboba@DESKTOP-T336VHB:~/biocomputing$` `echo` `"Number of A: $(grep -v "^>" Claudia.fasta | grep -o "A" | wc -l)"`

`echo` `"Number of G: $(grep -v "^>" Claudia.fasta | grep -o "G" | wc -l)"`

`echo` `"Number of T: $(grep -v "^>" Claudia.fasta | grep -o "T" | wc -l)"`

`echo` `"Number of C: $(grep -v "^>" Claudia.fasta | grep -o "C" | wc -l)"`
