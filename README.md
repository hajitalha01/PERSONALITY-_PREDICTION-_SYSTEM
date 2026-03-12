# PERSONALITY-_PREDICTION-_SYSTEM
Predict personality types from resumes (PDF/DOCX) using NLP and machine learning with OCEAN trait analysis.
# Resume Personality Predictor

A **Resume Personality Prediction System** that automatically predicts a candidate's **personality type** from their **resume (PDF or DOCX)** using **NLP** and **machine learning**. The system extracts the **Big Five (OCEAN) traits**, predicts personality, and visualizes results with interactive graphs.

---

## Features

- Upload **single resume** (PDF/DOCX)  
- Automatic **text extraction** from resumes  
- Detect **personal information** (Name, Age, Gender)  
- Extract **OCEAN (Big Five) trait scores**  
- Predict **personality type** using ML models:
  - Logistic Regression  
  - Random Forest  
  - Gradient Boosting  
- Visualize results:
  - Radar chart of OCEAN traits  
  - Bar charts of trait scores  
  - Prediction probabilities  
  - Candidate info card  
  - Model performance comparison  

---

## Pipeline Overview (8 Cells)

| Cell | Description |
|------|-------------|
| 1 | Install required Python libraries (`pdfplumber`, `python-docx`, `spaCy`, `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`) |
| 2 | Import libraries and load `spaCy` NLP model |
| 3 | Load training dataset, encode features, split train/test, scale data, train 3 ML models, select **best model** |
| 4 | Model evaluation: metrics comparison, confusion matrices, classification reports |
| 5 | Resume text extraction functions (PDF & DOCX) |
| 6 | NLP & OCEAN feature extraction, personal info detection, resume sections extraction |
| 7 | Visualization functions: radar charts, bar charts, prediction probabilities, candidate info card |
| 8 | Upload a single resume, analyze it, print results, show graphs |

---

## Quick Start

1. Open the notebook in **Google Colab**.  
2. Upload `resume_personality_app.ipynb`.  
3. Run **Cells 1–3** to install libraries, import them, and train ML models.  
4. Run **Cell 4** to visualize model evaluation.  
5. Run **Cells 5–6** to prepare resume extraction and feature extraction functions.  
6. Run **Cell 7** to prepare visualization functions.  
7. Run **Cell 8** to upload a **resume** and see the **predicted personality with graphs**.

---

## File Structure
├── training_dataset.csv # Training dataset for ML models
├── resume_personality_app.ipynb # Colab notebook with 8 cells
├── model_comparison.png # Model metrics visualization
├── confusion_matrices.png # Confusion matrices
├── resume_analysis_result.png # Resume analysis graphs
├── README.md # Project documentation


---

## Requirements

- Python 3.x  
- Google Colab recommended  
- Libraries:
  - `pdfplumber`  
  - `python-docx`  
  - `spaCy` (`en_core_web_sm`)  
  - `scikit-learn`  
  - `pandas`, `numpy`  
  - `matplotlib`, `seaborn`  

---

## Notes

- Supports **PDF and DOCX resumes**  
- Big Five traits are scored **1–10**  
- Best model is automatically selected based on **F1 Score**  

---

