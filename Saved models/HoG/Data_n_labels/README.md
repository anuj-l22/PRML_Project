The issue with extracting HoG features was that session's RAM was crashing and so we had split into part feature extractions , combine them and apply PCA which is time consuming so once applied it was stored for future use
- Syntax : <HoG_transformed_data>_<no_of_PCA_features>.joblib
- Also lables for future accuracy computation stored in labels.joblib
