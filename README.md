# Breast Cancer SML Project

This project is part of my Statistical Machine Learning coursework.  
It analyzes **breast cancer diagnosis** using features extracted from cell nuclei in fine needle aspiration (FNA) images of breast masses.

The repository contains:
- **`report.html`** – A redacted HTML report (first 5 lines of code shown, full code available in `src/`).
- **`src/`** – Source code for data processing, analysis, and model building.
- **Dataset description** – See below for feature explanations.

---

## 📊 Dataset Overview

Each row in the dataset represents a breast mass sample, with features computed from the FNA image of the cell nuclei.

### Features

1. **Radius** – Average distance between the nucleus center and its perimeter points. Larger radius may indicate malignancy.
2. **Texture** – Standard deviation of gray-scale values. Higher variation can signal irregular texture.
3. **Perimeter** – Total length around the nucleus.
4. **Area** – Total area of the nucleus. Malignant nuclei often have larger areas.
5. **Smoothness** – Local variation in radius lengths. Less smoothness means more irregularity.
6. **Compactness** – `(perimeter² / area) – 1`. Measures how compact the nucleus is.
7. **Concavity** – Severity of concave portions of the contour.
8. **Concave Points** – Number of concave points along the contour.
9. **Symmetry** – How symmetrical the nucleus is. Asymmetry can indicate malignancy.
10. **Fractal Dimension** – Complexity of the nucleus boundary.

For each feature, the dataset includes:
- **Mean** – Average over all measured nuclei in the sample.
- **Standard Error** – Variation across nuclei.
- **Worst (largest)** – Average of the three largest values, emphasizing extremes.

---

## 📂 Project Structure

```markdown

breast-cancer-sml-project/
│
├── src/                    # Source code 
│   ├── data_preprocessing.py  # Script for data 
│   ├── model_training.py      # Script for training
│   └── evaluation.py          # Script for model evaluation and metrics
│
├── report.html             # report 
├── README.md               # overview and setup
└── requirements.txt        # Python dependencies 

```
---

## 🚀 How to Run


#### 1. Clone the repository:

   ```bash
   git clone https://github.com/mortezamotegh/breast-cancer-sml-project.git
   cd breast-cancer-sml-project
   ```


#### 2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

#### 3. Run the analysis:
   ``` bash
  python src/data_preprocessing.py
  python src/model_training.py
  python src/evaluation.py
   ```


## 📜 License
This project is for educational purposes as part of a coursework submission.
Dataset used is from the UCI Machine Learning Repository:
https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)




