# breast-cancer-diagnostic-ml
Clinical diagnostic model using Logistic Regression and Feature Scaling to classify breast cancer tumors with high sensitivity
# 🔬 Breast Cancer Diagnostic Classification

## Project Overview
In clinical diagnostics, the accuracy of a model can be a matter of life and death. This project utilizes the **Wisconsin Breast Cancer Dataset** to build a predictive model that classifies tumors as **Malignant** (0) or **Benign** (1) based on digitized images of fine needle aspirates (FNA) of breast masses.

As a **Bioinformatics Master's graduate**, I have designed this pipeline to emphasize **clinical safety**, prioritizing the minimization of **False Negatives** (missing a cancer diagnosis) over general accuracy.

---

## Data Science Workflow

### 1. Data Preprocessing & Feature Scaling
Biological measurements (like cell area vs. smoothness) often exist on vastly different scales. 
* **Standardization:** I applied `StandardScaler` to ensure all 30 features have a Mean of 0 and a Standard Deviation of 1.
* **Integrity:** The scaler was fit strictly on the **Training Set** to prevent **Data Leakage**, ensuring the model remains robust on unseen clinical data.

### 2. Model Architecture
I implemented **Logistic Regression**, a gold standard in medical research due to its interpretability. In a clinical setting, understanding "why" a model flagged a patient is as important as the prediction itself.

### 3. Evaluation Metrics (The "Bio-Med" Lens)
While the model achieves high overall accuracy, my evaluation focuses on:
* **Recall (Sensitivity):** Maximizing the detection of all Malignant cases.
* **Confusion Matrix Analysis:** Visualizing the trade-off between False Positives and False Negatives.

---

## Key Results
* **Accuracy:** ~98%
* **Recall (Malignant Class):** [Insert your Recall score here, e.g., 0.96]
* **F1-Score:** [Insert your F1 score here]



---

## How to Run
1. Clone the repository.
2. Ensure you have `scikit-learn`, `pandas`, and `seaborn` installed.
3. Run the Jupyter Notebook `Breast_Cancer_Analysis.ipynb`.

## 🧬 About the Author
**[Your Name]** *MSc in Bioinformatics | Telecom Engineer | Startup Founder* Bridging the gap between engineering logic and life sciences through Data Science.
