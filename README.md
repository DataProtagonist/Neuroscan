# Neuroscan
# Parkinson's Disease Detection Using Machine Learning 🎯

This repository contains the full implementation of the Parkinson's Disease Detection project, leveraging vocal features and the XGBoost algorithm to create a highly accurate, non-invasive diagnostic tool for early detection of Parkinson's disease.

## 📂 Project Overview

The project employs machine learning techniques, particularly the **XGBoost** algorithm, to analyze vocal characteristics such as jitter, shimmer, and harmonic-to-noise ratio (HNR) for detecting early signs of Parkinson's disease. The goal is to provide medical professionals with a user-friendly, non-invasive tool that can aid in early diagnosis.

The system includes a web interface where users can input their vocal data and receive an immediate prediction, helping clinicians identify potential Parkinson's cases.

## 🚀 Project Goals

- Achieve an accuracy rate of over **90%** using vocal biomarkers.
- Provide an accessible, non-invasive method to detect early Parkinson’s disease.
- Develop a scalable system that can be used by medical professionals to improve patient outcomes.

## ⚙️ Technologies & Tools

- **Machine Learning**: XGBoost, Scikit-learn
- **Languages**: Python (for model development), HTML/CSS/JavaScript (for the web interface)
- **Frameworks**: Flask (backend), Bootstrap (for frontend styling)
- **Cloud**: Jupyter notebooks for prototyping
- **Data Handling**: Pandas, NumPy
- **Data Visualization**: Matplotlib

## 📊 Dataset

The dataset includes vocal recordings from patients diagnosed with Parkinson's disease and healthy individuals. These recordings were processed and features such as jitter, shimmer, and HNR were extracted for analysis.

- `ProcessedPDDdata.xlsx`: Contains processed features from vocal recordings, including jitter, shimmer, and HNR.

## 🧠 Machine Learning Model

- **Algorithm**: We employed the **XGBoost** classifier for its robustness in classification tasks, particularly in handling complex, imbalanced datasets like medical data.
- **Performance**: The model achieved a **97% accuracy** in detecting Parkinson's disease based on vocal features. Key metrics such as precision, recall, and F1-score were used to evaluate the model's performance.

### Model Parameters
- **Number of Trees**: 100
- **Max Depth**: 2
- **Learning Rate**: 0.3
- **Evaluation Metric**: Classification error

See the `xgbclassifier.json` for full model parameters.

## 🖥️ Web Interface

The system includes a web-based interface that allows users (e.g., neurologists) to input vocal measurements and receive predictions in real-time.

- **Input Fields**: Users input features such as `MDVP:Fo(Hz)`, `MDVP:Shimmer`, and `NHR` (Noise-to-Harmonic Ratio) to make predictions.
- **Results**: The prediction page displays a clear output indicating whether Parkinson's disease is detected or not.

## 📈 Performance & Testing

- **Accuracy**: 97%
- **Precision**: High sensitivity to detect early-stage Parkinson's.
- **F1 Score**: Optimized for balanced precision and recall.
  
## 📅 Project Timeline

| Task                        | Duration      |
|-----------------------------|---------------|
| Data Collection              | 8 days        |
| Data Preprocessing           | 7 days        |
| Model Development            | 15 days       |
| Testing and Evaluation       | 14 days       |
| Final Review and Documentation| 4 days       |

## 📂 Directory Structure

parkinsons-disease-detection/ │ ├── data/ # Processed data and datasets ├── model/ # Saved models and configuration files ├── notebooks/ # Jupyter notebook for the full workflow ├── scripts/ # Python script for training and inference ├── web/ # Frontend and backend files for the web interface └── README.md # Documentation of the project


## 💻 Usage Instructions

1. Clone the repository:
  ```bash
  git clone https://github.com/DataProtagonist/parkinsons-disease-detection.git
  ```
2. Install Dependencies
  ```bash
  pip install -r requirements.txt
  ```
3. Run the web app locally:
  ```bash
  python app.py
  ```
4. Access the web interface at **"http://localhost:5000"**.
