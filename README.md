# Continuous Feature Representations for FT-Transformers in Tabular Data

Deep learning models based on the Transformer architecture have recently been adapted for tabular data, but their performance often depends on how numerical features are represented.

This project evaluates several numerical feature representations for the **FT-Transformer** and examines their effect on predictive performance across multiple tabular datasets. We compare four representations applied before the model’s feature-specific embedding layer:

- Raw scalar inputs  
- Z-score normalization  
- Rank-based representation (proposed)  
- Piecewise Linear Encoding (PLE)

Experiments were conducted on six tabular datasets from Kaggle/UCI and a clinical dataset of septic shock patients from Sheba Medical Center. Model performance was evaluated using **ROC-AUC**, and results were compared to a **Random Forest baseline**.

Overall, the results show that numerical feature representation can influence FT-Transformer performance. PLE often achieved the strongest results among the FT-Transformer methods, while Random Forest models remained competitive and required substantially less training time. Yet, no significant difference was found between the methods.

## Authors

Shiri K. Nitzan-Tzahor
Yonatan Seleznev  

## Files

- `DL_proj_report_Shiri_Yonatan_FTTransformers.pdf` – full project report  
- `DL_proj_code_Shiri_Yonatan_FTTransformers.ipynb` – project code
