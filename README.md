# LMPred: Predicting Antimicrobial Peptides Using Pre-Trained Language Models and Deep Learning

## Abstract (Taken from Dissertation Report)
Antimicrobial peptides (AMPs) are increasingly being used in the development of new therapeutic drugs, in areas such as cancer therapy and hypertension. Additionally, they are seen as an alternative to antibiotics due to the increasing occurrence of bacterial resistance. Wetlaboratory experimental identiﬁcation, however, is both time consuming and costly, so in-silico models are now commonly used in order to screen new AMP candidates. This paper proposes a novel approach of creating model inputs; using pre-trained language models to produce contextualized embeddings representing the amino acids within each peptide sequence, before a convolutional neural network is then trained as the classiﬁer. The optimal model was validated on two datasets, being one previously used in AMP prediction research, and an independent dataset, created by this paper. Predictive accuracies of 93.33% and 88.26% were achieved respectively, outperforming all previous state-of-the-art classiﬁcation models.

## Files Uploaded:
- LM_Pred_Dataset Folder contains the training, validation and test set independently sourced and used in the research paper as the "LMPred" dataset.
- 1_Create_Word_Embeddings.ipynb shows an example of how to create embeddings using the pre-trained language models (in this case T5XL Uniref50), inputting amino acid sequences of AMPs and Non-AMPs and outputting vectorized embeddings.
- 2_Build_CNN_Model.ipynb shows how the convolutional neural network models were built that used the word embedding vectors in order to classify peptide sequences. 
- 3_Testing_Models.ipynb shows the testing of the built models on the unseen test data. Data from external webserver model predictions is incorporated. 
