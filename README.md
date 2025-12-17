# 🧠 AI-Powered Alzheimer’s Progression Analysis

> **Hack4Health 2025 Submission** > *Early Detection & Interpretability using Deep Learning & SHAP*

## 📌 Project Overview
Alzheimer's disease affects millions, yet its progression is often subtle in early stages. This project utilizes a **Convolutional Neural Network (CNN)** to classify MRI scans into four stages of dementia. Crucially, we move beyond "Black Box" predictions by integrating **SHAP (SHapley Additive exPlanations)** to visualize exactly *where* the AI is looking—validating that our model identifies biological markers like ventricular enlargement and hippocampal atrophy.

## 🚀 Key Features
* **Multi-Class Classification**: Detects 4 stages: *Non-Demented, Very Mild, Mild, and Moderate*.
* **Fast & Efficient**: Optimized training pipeline (Parquet data handling + Custom Data Generators).
* **Explainable AI (XAI)**:
    * **Saliency Maps**: Individual patient "Heatmaps" showing critical brain regions.
    * **Global Pattern Discovery**: Aggregated attention maps revealing disease progression patterns.
* **Medical Metrics**: Evaluated using **ROC-AUC** curves and per-class Sensitivity/Recall.

## 🛠️ Tech Stack
* **Deep Learning**: TensorFlow/Keras (CNN Architecture)
* **Data Handling**: Pandas, PyArrow (Parquet format)
* **Explainability**: SHAP (GradientExplainer)
* **Visualization**: Matplotlib, Seaborn

## 📊 Results & Visualizations

| **Confusion Matrix** | **ROC Curves** |
|:---:|:---:|
| <img src="images/confusion_matrix.png" width="300"> | <img src="images/roc_curve.png" width="300"> |

### 🧠 The "Brain Map" (Explainability)
Our model autonomously learned that **enlarged ventricles** (the dark center gaps) are key indicators of Moderate Dementia.

<img src="images/winning_brain_patterns.png" width="800">

## 📥 Installation & Usage

1.  **Clone the Repo**
    ```bash
    git clone [https://github.com/your-username/alzheimers-ai-shap.git](https://github.com/your-username/alzheimers-ai-shap.git)
    cd alzheimers-ai-shap
    ```

2.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebook**
    Open `AI_4_Alzheimer_SHAP_Visulizations.ipynb` in Jupyter or Google Colab.

## 📂 Dataset
The model utilizes a de-identified MRI dataset (Parquet format) containing pre-processed, skull-stripped brain scans labeled by clinical severity.

## 🏆 Hackathon Context
This project was built for **Hack4Health**, focusing on the **Interpretability** track. We demonstrate that AI can be a *transparent* clinical support tool, not just a prediction engine.

---
*Built with ❤️ by [Your Team Name]*
