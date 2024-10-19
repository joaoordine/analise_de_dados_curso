# analise_de_dados_curso
Repositório destinado à realização das listas de exercícios e do projeto final referente à disciplina RBP5802 - Introdução à ciência dos dados.


# Final Project 
## *Prediction of Alternative Open Reading Frames (Alt-ORFs) in a model breast cancer cell line (MCF7)*
"Transcriptional and post-transcriptional mechanisms diversify the proteome beyond gene number while maintaining a sequence relationship between original and altered proteins. A new mechanism breaks this paradigm, generating novel proteins by translating alternative open reading frames  (Alt-ORFs) within canonical host mRNAs." Using bioinformatic pipelines to predict Alt-ORFs within a genome can be helpful to proteomics, allowing the identification of novel proteins within the same proteomic data using simply the MS database. Hereinafter are the scripts used to process genomic data from public databases (WGS) from a widely used breast cancer cell line, namely MCF7 and in the prediction of Alt-ORFs within this genome. 

### Genome Retrieval and Processing
*Option 1*: Ben-David, U., Siranosian, B., Ha, G. et al. Genetic and transcriptional evolution alters cancer cell line drug response. Nature 560, 325–330 (2018). https://doi.org/10.1038/s41586-018-0409-3 - BioProject PRJNA398960; MCF7-scWT5-TS (SRR6730014)
Check script 01.Process_WGS_NCBI.ipynb

*Option 2*: Deng, N., Minoche, A., Harvey, K. et al. Deep whole genome sequencing identifies recurrent genomic alterations in commonly used breast cancer cell lines and patient-derived xenograft models. Breast Cancer Res 24, 63 (2022). https://doi.org/10.1186/s13058-022-01540-0 - European Genome Archive (accession number EGAS00001006285)

### Predicting Alt-ORFs 
Check script 02.Alt-ORF_Prediction.ipynb

### Processing ORFs output 
- Translating nucleic acid sequences from Alt-ORFs to amino acid sequences
Check script 03.Translate_seqs.ipynb

- In silico trypsin digestion of protein sequences (simulate sample treatment before MS)
Check script 04.Trypsin_digestion.ipynb

### Visualize generated Alt-ORFs  
Biopython might be interesting --> - descriptive statistics Alt-ORFs
- Plots: bar charts with counts, longest-to-smallest ORFs, codon/ORF preference etc
