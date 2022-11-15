2022-11-10

Transmembrane topology prediction of Yvc1 and Flc2 homologs using two independent methods. 

1. DeepTMHMM  https://doi.org/10.1101/2022.04.08.487609

I used DeepTMHMM to predict the transmembrane topology of Flc2 homologs and Yvc1 homologs. I used the DeepTMHMM web server https://dtu.biolib.com/DeepTMHMM which takes protein sequences in fasta format and outputs results as a .gff3 file. 

I saved the results as "Flc2_hits_DeepTMHMM.gff3" and "Yvc1_hits_DeepTMHMM.gff3". Each file was edited by removed trailing tabs and replacing "//" with "#" to make data processing in R easier. 


2. TMbed https://doi.org/10.1186/s12859-022-04873-x

I used the Google Colab notebook https://colab.research.google.com/drive/1FbT2rQHYT67NNHCrGw4t0WMEHCY9lqR2?usp=sharing which I found through the developer's GitHub https://github.com/BernhoferM/TMbed. It takes protein sequences in fasta format and returns a .txt file in 3-line format or a tabular file with topology probabliles per residue. I downloaded both output formats and saved as 

"Flc2_predictions_TMbed_3line.txt"
"Flc2_predictions_TMbed_tabular.txt"
"Yvc1_predictions_TMbed_3line.txt"
"Yvc1_predictions_TMbed_tabular.txt"