# Phage-Host_Codon_Compatibility
Repo for Phage-Host Codon Compatibility Pipeline

## Dependenices:

Pyhton 3 -- https://www.python.org/downloads/

BioPython -- https://biopython.org/wiki/Download

R -- https://www.r-project.org/

Pandas -- https://pandas.pydata.org/

SciPy -- https://scipy.org/install.html


## **Instructions:**

1. Download all files into a directory

2. Navigate to the directory containing the the downloaded repo files

3. Execute the command: python3 wrapper.py -s XXX -q XXX
        
        Arguments:
        
        -s AA012345.1    (RefSeq Accession of bacterial genome or file path to bacterial CDS fasta file)
        -q A01234.1      (RefSeq Accession of phage genome or file path to phage CDS fasta file)


**Files used for testing:**
    
    Bacteria 1 (ECBacteria.txt) -- E. coli K12 strain C3026; RefSeq Accession: CP014272.1
    Bacteria 2 (SPBacteria.txt -- Streptococcus pneumoniae AP200; RefSeq Accession CP002121.1
    Phage 1 (ECPhage.txt) -- Escherichia phage lambda; RefSeq Accession: J02459.1
    Phage 2 (LPPhage.txt) -- Lactobacillus plantarum bacteriophage LP65; RefDeq Accession: AY682195.1

**Test Runs:**

    Positive Control: python3 wrapper.py -s CP014272.1 -q J02459.1
    Negative Control (Bacteria): python3 wrapper.py -s CP002121.1 -q J02459.1
    Negative Control (Phage): python3 wrapper.py -s CP014272.1 -q AY682195.1
