# Explainable-ML-Based-Distinguisher-of-Stream-Ciphers-using-Boosting-and-Transformer
This project presents a machine learning framework to distinguish cryptographic keystreams from truly random bitstreams using two different models:
1.XGBoost Classifier
2.Transformer-based Neural Network with Self-Attention
Further, Explainable AI (XAI) techniques such as SHAP and LIME are applied to interpret the predictions made by the XGBoost model.

# Datasets:
- Keystreams: Generated using stream cipher algorithms (1.csv, 2.csv, 3.csv, 4.csv)
- Random Streams: Truly random bitstreams (random_streams.csv)
- Binary classification labels:
  -1 for keystream
  -0 for random stream

# Models Used:
# 1. XGBoost Classifier
- A gradient boosting algorithm optimized for performance on tabular data.
- Achieved up to 73.58% accuracy, significantly outperforming the Transformer model.
- Fast execution (~1 minute per dataset).

# 2. Transformer-based Model
- Utilized self-attention, normalization, and dense layers.
- Accuracy plateaued around 49.53%, indicating random performance.
- Computationally heavy (3–4 minutes per run).

# Explainability with SHAP and LIME
# 1. SHAP (SHapley Additive exPlanations)
- Provided global feature importance and local instance-level interpretation.
- Offered consistent, additive, and theoretically grounded explanations.
- Executed faster and yielded more reliable results.

# 2. LIME (Local Interpretable Model-agnostic Explanations)
- Focused on local interpretability.
- Helped visualize the contribution of each feature for a single prediction.
- Had a lower fidelity score (R² ≈ 0.0138) and longer runtime.
