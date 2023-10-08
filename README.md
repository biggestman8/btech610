### Lab 6 Reproducible
**Author**: Jian  
**Date**: 14/10/23


This is my first Markdown code file! 

##### I can make a numbered list:  
1. item 1  
2. item 2  
3. item 3  

##### I can make an unnumbered list: 
- item 1 
- item 2 
- item 3 

##### I can make a table:
| col1 | col2 | col3 |  
| ---- | ---- | ---- |  
| DNA  | DNA  | DNA  |  
| Genetic Code | Transcripts | Peptide |  
| Double Helix | Single Strand | Alpha Helix |  

##### Python example 
```python
#!/usr/bin/python3
import sys
from Bio import SeqIO
from Bio.SeqUtils import GC 

def parse_fasta_file(fasta_file_path): 
    sequences = SeqIO.parse(fasta_file_path, "fasta")
    for seq_record in sequences:
        print (seq_record.id, len(seq_record), round(GC(seq_record.seq), 2))

if __name__ == "__main__":
    parse_fasta_file(sys.argv[1])
```

##### Shell code block example 
```sh
mkdir lab6
cd lab6 
touch README.md
```

EOF :)