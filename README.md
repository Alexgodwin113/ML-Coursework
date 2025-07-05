# 🩺 Breast Ultrasound Image Classification using Deep Learning

This project focuses on building an **automated classification system** to distinguish between **malignant** and **benign** breast tumors using ultrasound images. The system leverages deep learning techniques and optimization strategies to enhance model performance and support early diagnosis.

## 📌 Project Summary

Breast cancer remains a global health issue, where early and accurate diagnosis is key. This project utilizes **ResNet-based architectures** to classify breast ultrasound images. Various strategies such as **hyperparameter tuning**, **architectural modifications**, and **data transformations** were applied to improve performance beyond baseline results.

## 🧪 Dataset

- **BreastMNIST**: 28x28 grayscale breast ultrasound images
- Categories: Malignant vs. Benign
- Source: [Breast Ultrasound Dataset](https://www.nature.com/articles/s41597-024-02984-z)

## 🚀 Model Development

- **Baseline Model**: ResNet-18 (Pretrained on ImageNet)
- **Improvements Made**:
  - Architectural modifications to ResNet18
  - Custom loss functions
  - Seed function for reproducibility
  - Learning rate optimization using **Optuna**
  - Hyperparameter tuning via grid search

## 📈 Performance

| Metric                | Baseline | Final Model |
|-----------------------|----------|-------------|
| Accuracy (Test Set)   | 0.863    | 0.8767      |
| AUC (Test Set)        | 0.901    | 0.9105      |
| AUPR                  | —        | 0.9238      |
| F1 Score              | —        | 0.8821      |
| 5-Fold CV Accuracy    | —        | 0.8040      |
| 5-Fold CV AUC         | —        | 0.8123      |

## 🧠 Key Concepts

- **AUC vs Accuracy**: AUC reflects model’s ranking ability; higher AUC indicates better class separation.
- **AUPR vs F1 Score**: AUPR balances precision and recall across thresholds; F1 measures harmonic mean.
- **Cross-validation**: Used for robust performance estimation and to reduce variance from single test splits.

## 📚 Literature Insights

- Early approaches relied on feature engineering + SVMs.
- CNNs like ResNet have outperformed traditional methods.
- ResNet18 showed better performance than ResNet50 on BreastMNIST in prior studies.

## 🛠 Tools & Technologies

- Python
- PyTorch
- Optuna
- Scikit-learn
- Matplotlib/Seaborn for evaluation

## 📎 References

- [Deep Residual Learning (He et al., 2016)](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)
- [BreastMNIST Dataset - Nature](https://www.nature.com/articles/s41597-024-02984-z)
- [Ultrasound Classification Research (2022)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8840464/)

## 🙌 Acknowledgements

This work was carried out as part of an independent research project aimed at applying AI in healthcare to support early cancer detection through improved diagnostic models.

---

*Feel free to contribute, report issues, or fork this repo to build upon it.*
