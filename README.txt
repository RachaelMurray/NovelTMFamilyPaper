2022-11-10

Jackhmmer directory:

I performed searches for homologs of S. cerevisiae Flc2 and S. cerevisiae Yvc1 against the proteomes of 4 fungal species 

- A. fumigatus
- S. cerevisiae
- S. pombe
- C. neoformans

1. I retrieved the taxon ID numbers for these species from the NCBI taxonomy browser website https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi and saved them in the file "taxon_ids_structural_comparison.txt"


2. I downloaded the protein sequences of S. cerevisiae Flc2 and S. cerevisiae Yvc1 in fasta format from uniprot https://www.uniprot.org and saved them as "S.cerevisiae_Flc2_P39719.fasta" and "S.cerevisiae_Yvc1_Q12324.fasta"
 

3. I performed jackhmmer searches for each query protein using the ebi HMMER web server at https://www.ebi.ac.uk/Tools/hmmer/search/jackhmmer
I set the sequence database to UniprotKB and used restricted the search to the 4 species listed above using their taxon IDs. Default cut-off parapets were used. I performed multiple iterations until no more unique sequences were returned and saved the results from the final iteration in .tsv format as "Flc2_jackhmmer_iteration3_hits.tsv" and "Yvc1_jackhmmer_iteration1_hits.tsv". 

4. I could not download protein sequence hits is fasta format from jackhmmer, instead I copies the target accession identifies from "Flc2_jackhmmer_iteration3_hits.tsv" and "Yvc1_jackhmmer_iteration1_hits.tsv" and used the uniprotID mapping tool to find the sequences in the uniprotKB database https://www.uniprot.org/id-mapping
I downloaded the protein sequences in fasta format and saved them as "Flc2_jackhmmer_iteration3_sequences.fasta" and "Yvc1_jackhmmer_iteration1_sequences.fasta". I also downloaded the default information associated with the protein entries and saved in .tsv format as "Flc2_jackhmmer_iteration3_uniprot_info.tsv" and "Yvc1_jackhmmer_iteration1_uniprot_info.tsv" 




