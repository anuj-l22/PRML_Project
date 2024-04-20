Directory Structure : 
- CNN folder consists of training codes on PCA reduced CNN features
- HoG folder consists of training codes on PCA reduced HoG features
- LBP folder consists of training codes on PCA reduced LBP features
- Accuracies folder consists of codes using pickled models to check accuracies and report them
- PRML_Feat_ext.ipynb notebook is the one used for extracting CNN , HoG and LBP features , any explicit usage instruction is mentioned in notebook otherwise it can be run directly as it uses wget to link dataset to notebook and accordingly code is prepared
- Usage instruction :
   - Firstly the PRML_Feat_ext code needs to be runned to save the extracted features locally
   - Then the training notebooks in CNN/HoG/LBP have code for face extraction
   - As there are multiple .pt files for HoG , its faces are extracted , PCA transformed and stored in Saved_models
