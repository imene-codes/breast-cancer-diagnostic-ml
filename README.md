# breast-cancer-diagnostic-ml
Clinical diagnostic model using Logistic Regression and Feature Scaling to classify breast cancer tumors with high sensitivity
# Breast Cancer Diagnostic Classification

## Project Overview
This project applies Machine Learning to clinical oncology. Using the Wisconsin Breast Cancer dataset, I built a model to classify tumors as Malignant (Cancerous) or Benign (Healthy).
# The Bioinformatics Context In medical diagnostics
The cost of a False Negative (telling a sick patient they are healthy) is catastrophic. Therefore, this project prioritizes Recall and utilizes Feature Scaling to ensure that small-scale biological measurements (like "smoothness") are weighted equally against large-scale measurements (like "area").

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
