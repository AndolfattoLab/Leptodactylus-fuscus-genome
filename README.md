# Leptodactylus-fuscus-genome
The *de novo* genome assembly of *Leptodactylus fuscus*


This presents a *de novo* genome assembly of *Leptodactylus fuscus*. High molecular weight DNA was extracted from a *L. fuscus* embryo which had been preserved in ethanol upon collection in Garzón, Huila, Colombia. The library was prepared and sequenced with 10X Genomics Chromium. Linked reads were propessed by Long Ranger basic v2.2.2 and assembled with Supernova v2.1.1. The assembled genome is 2.42 Gb with 16,530 scaffolds >=10 kb, and scaffold N50 = 363 kb. The assembly size of contigs larger than 10 kb (1.26 Gb) is about half of the estimated genome size (2.4 Gb). 72.6% of the BUSCO Tetrapoda gene annotations (version odb10) were identified.


## Methods
High-molecular-weight genomic DNA was isolated from a single *Leptodactylus fuscus* individual and used to prepare a 10x Genomics Chromium library that was sequenced on Illumina HiSeq X sequencer (HudsonAlpha Institute of Biotechnology, Alabama, USA.). 
Barcodes were removed using the Long Ranger basic v2.2.2 (https://support.10xgenomics.com/genome-exome/software/downloads/latest). 
Trimmed reads were used for k-mer estimation in Jellyfish (v2.2.7). The k-mer (k=21) frequency distribution was processed in GenomeScope to estimate the genome size, heterozygosity, and percentage of repeat content. 
The linked-reads were assembled using the Supernova v2.1.1 assembler using default settings and the “–accept-extreme-coverage” flag. 
A summary of the assembly is provided in the Table S3 of the associated publication. 
The assembled genome is 2.42 Gb (16,530 scaffolds >=10 kb, scaffold N50 = 363 kb) and was outputted in the pseudohap2 format. The assembly size of contigs larger than 10 kb (1.26 Gb) is only ~1/2 of the estimated genome size (2.4 Gb). 
The completeness of the genome assembly was assessed using Benchmarking Universal Single-Copy Orthologs (BUSCOs, v4.0.5), and 72.6% of the BUSCO Tetrapoda gene annotations (version odb10) were identified.


## Notes
1. The assembly is outputted in the pseudohap2 format. Other formats like megabubbles and pseudohap are also available upon request. 
2. The coverage of this genome to be ~50X which is within the recommended sequencing depth of 38-56X coverage. However, a flag "--accept-extreme-coverage" was used for assembling because dropping it caused the assembler to crash. While we tested other methods, like increasing the memory, only adding –accept-extreme-coverage seemed to resolve the issue. 


## Citation
Mohammadi, S.1, Yang, L.1, Harpak, A.1, Herrera-Álvarez, S., Rodríguez-Ordoñez, M., Peng, J., Zhang, K., Storz, J., Dobler, S., Crawford, A. and Andolfatto, P., 2020. Concerted evolution reveals co-adapted amino acid substitutions in Na+K+-ATPase of frogs that prey on toxic toads. *biorxiv*. doi: https://doi.org/10.1101/2020.08.04.234435 (1: these authors contribute equally).
