# <img src="https://github.com/user-attachments/assets/1eaeaf5c-081d-4d76-b816-bca55d979ad3" width="100">  3DisoTransFold

"3DisoTransFold" pipeline was used to evaluate translation ORFs and predict isoform structures across transcriptome-identified transcripts, ultimately constructing a protein structural similarity network, “3DisoGalaxy,” based on multiple structure alignment scores comparing isoform structures. Specifically, the predicted ORFs from the master transcriptome were retained only if identified by Ribo-seq analysis, supporting their participation in the translation process.
![image](https://github.com/user-attachments/assets/95735db2-8587-4723-8673-71b440dadeb1)

By combining BLASTP and HMMER methods, ORF sequences were predicted using TransDecoder and machine learning. After filtering out low-confidence and short ORFs, the longest ORF sequence was kept for each isoform, and AlphaFold-2.3 was utilized to predict protein structures. Structural similarity was then calculated using the TMalign method, collecting pairwise isoform similarities to construct a “protein universe.” Additionally, functional domains and GO term pathway annotations were assigned to the network based on UniProtKB databases.

# 3DisoGalaxy & 3DisoTranFold
The pipeline <img src="https://github.com/user-attachments/assets/1eaeaf5c-081d-4d76-b816-bca55d979ad3" width="100"> [https://github.com/CityUHK-CompBio/TranStructomics](https://github.com/CityUHK-CompBio/3Diso-TransFold), was used to evaluate translation ORFs and predict isoform structures across transcriptome-identified transcripts, ultimately constructing a protein structural similarity network, “3DisoGalaxy,” based on multiple structure alignment scores comparing isoform structures. Specifically, the predicted ORFs from the master transcriptome were retained only if identified by Ribo-seq analysis, supporting their participation in the translation process.  




By combining BLASTP and HMMER methods, ORF sequences were predicted using TransDecoder and machine learning. After filtering out low-confidence and short ORFs, the longest ORF sequence was kept for each isoform, and AlphaFold-2.3 was utilized to predict protein structures. Structural similarity was then calculated using the TMalign method, collecting pairwise isoform similarities to construct a “protein universe.” Additionally, functional domains and GO term pathway annotations were assigned to the network based on UniProtKB databases.  

Through the final network, the landscape of cancer-specific alternative splicing-induced protein isoforms becomes available, allowing for the screening and validation of subtype-specific isoforms for therapeutic applications. 

A case study version of the final network, **“3DisoGalaxy”**, can be accessed at  
<a href="http://hkwanglab-compbio.com:3831/">
    <img src="https://github.com/user-attachments/assets/d02384b5-b85f-4716-b657-7a122ca92d02" width="100">
</a>  
and the **“3DisoTransFold”** pipeline for analyzing all data is available at  
<a href="https://github.com/CityUHK-CompBio/3Diso-TransFold">
    <img src="https://github.com/user-attachments/assets/1eaeaf5c-081d-4d76-b816-bca55d979ad3" width="100">
</a>
