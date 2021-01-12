# Point mutation identification

Quick identification and summary of mutations in a sequence compared to a reference sequence.

This is a function written in Python to identify point mutations in a coding sequence aligned to a reference sequence, with subsequent alterations to amino acid sequence identified. The script has been designed with plasticity and enables the user to print a number of desired outputs including: anti-sense, mRNA, seperated codons and amino acid sequences in both 3-letter and single-letter formats. 

The example data provided can be used to run the script. It explores point mutations in a codon-optimized GFP for the plant pathogen *Zymospetoria tritici.*

To run:

1. Download Python scripts and example data files (eGFP.txt and ZtGFP.txt) into a single directory.

2. Run the script and check the alignment score is as expected (an alignment score of 0 indicates that the data inputs align at the first base and is expected with the example dataset). The printed sequence "reference:" and "mutated:" are the output from the search tool that identifies the start codon 'ATG' and trims prior nucleotides. Optimal data input has an alignment score of 0 and begins at the start of the coding sequence (open reading frame).

3. The data goes through a series of conversions, of which can be printed for desired outputs as mentioned above. Simply remove the '#' where indicated.

4. There are two output tables in this script. The first displays differences in nucleotide bases (DNA displayed) at specified positions, corresponding changes to the codon and if there is a change to the amino acid. No change to the amino acid will display as blank. The example data has 54 silent point mutations, so no amino acid changes will be observed in the last two columns. The second table is a short summary, displaying the number of point mutations and the number of amino acid changes (if any).


Appendix

Example data text files of eGFP and ZtGFP were transcribed from Kilaru et al (2015) A codon-optimized green fluorescent protein for live cell imaging in *Zymoseptoria tritici. Fungal Genetics and Biology.* **79** pp.125-131. doi: 10.1016/j.fgb.2015.03.022.

Script was written in Python 3.8.5
