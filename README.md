# Data Science / Machine Learning Projects(Internship tasks)

A collection of three end-to-end Data Science & ML projects covering biomedical signal analysis, neuroscience visualization, and agricultural AI.

---

## Repository Structure

```
ds-ml-projects/
├── task1_prosthetic_analysis/
│   ├── prosthetic_performance_analysis.ipynb
│   └── emg_usage_dataset.csv              ← generated on first run
├── task2_eeg_visualization/
│   └── eeg_data_visualization.ipynb
├── task3_crop_recommendation/
│   ├── crop_recommendation_system.ipynb
│   └── crop_recommendation_dataset.csv    ← generated on first run
├── requirements.txt
└── README.md
```

---

## Task 1: Prosthetic Performance Analysis

**Dataset:** Simulated EMG/usage dataset  
**Goal:** Analyze the relationship between prosthetic accuracy and user comfort

### What it does
- Simulates a realistic EMG dataset (200 users, 3 prosthetic types)
- Analyzes accuracy vs user comfort trade-offs
- Explores impact of user experience, EMG signal quality, and prosthetic type
- Generates a **multi-panel insights dashboard**

### Key Features
| Feature | Description |
|---|---|
| EMG RMS | Root Mean Square of EMG signal intensity |
| Accuracy | Gesture recognition accuracy (%) |
| Comfort Score | User-rated comfort (1–10 scale) |
| Prosthetic Type | Myoelectric / Body-Powered / Hybrid |

### Output
- `prosthetic_insights_dashboard.png` — 8-panel visualization

---

## Task 2: EEG Data Visualization

**Goal:** Plot and interpret brainwave patterns across all frequency bands

### Brainwave Bands Covered
| Band | Frequency | State |
|---|---|---|
| Delta | 0.5–4 Hz | Deep sleep |
| Theta | 4–8 Hz | Drowsiness, meditation |
| Alpha | 8–13 Hz | Relaxed wakefulness |
| Beta | 13–30 Hz | Active thinking |
| Gamma | 30–100 Hz | High-level cognition |

### Output
- `eeg_brainwave_charts.png` — Raw signal, per-band plots, PSD, band power comparison
- Clinical interpretation of dominant brainwave bands

---

## Task 3: Crop Recommendation System

**Dataset:** Simulated Crop Recommendation Dataset (based on UCI benchmark)  
**Goal:** Predict the best crop to grow based on soil nutrients and weather

### Features Used
| Feature | Unit | Description |
|---|---|---|
| N | mg/kg | Nitrogen content |
| P | mg/kg | Phosphorus content |
| K | mg/kg | Potassium content |
| Temperature | °C | Ambient temperature |
| Humidity | % | Relative humidity |
| pH | — | Soil pH |
| Rainfall | mm | Annual rainfall |

### Models Trained
- **Random Forest** (best performer)
- Decision Tree
- Naive Bayes

### Output
- Trained model: `crop_recommendation_model.pkl`
- Evaluation charts: confusion matrix + feature importance
- `recommend_crop()` function for real-time predictions

---

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/ds-ml-projects.git
cd ds-ml-projects
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

Open any notebook inside its task folder and run all cells (`Kernel → Restart & Run All`).

---

## Tech Stack

- **Python 3.10+**
- **Jupyter Notebook**
- pandas, NumPy, SciPy
- Matplotlib, Seaborn
- scikit-learn

---

## Sample Outputs

| Task | Output Preview |
|---|---|
| Task 1 | 8-panel dashboard: accuracy/comfort scatter, heatmap, distributions |
| Task 2 | Raw EEG signal, 5 band plots, PSD spectrum, band power bar chart |
| Task 3 | Confusion matrix, feature importance, per-crop recommendations |

---

## License

MIT License — free to use and modify.
