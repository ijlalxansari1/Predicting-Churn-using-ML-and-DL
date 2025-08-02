## 📊 User Churn Prediction with Ethical Insights

**Bachelor’s Thesis Research | SLAM 2018 Dataset**
Author: *Your Name*
Status: **\[In Progress]**

---

### 📘 Overview

This project investigates **user churn prediction** across social media platforms using the SLAM 2018 dataset. In addition to traditional behavioral modeling, it uniquely integrates **attention engineering**, **digital ethics**, and **data governance** into the machine learning pipeline.

The project is structured as a reproducible data science pipeline using Python and Jupyter Notebooks. It aims to go beyond basic churn prediction by raising critical questions:

* *What behavioral signals precede user dropout?*
* *Are we ethically modeling attention and engagement?*
* *How can churn insights be responsibly designed?*

---

### 🧠 Research Objectives

1. **Model churn behavior** across TikTok, YouTube, Instagram, Twitter, and Snapchat.
2. **Engineer time-based and session-based features** from raw event data.
3. **Develop predictive models**, including Logistic Regression, Random Forest, and LSTM.
4. **Integrate ethical considerations**, such as digital attention, informed consent, and behavioral surveillance.
5. **Visualize churn behaviors** across user types, clients, and platforms.
6. **Support ethical-by-design feature development** in user-facing platforms.

---

### 📁 Project Structure

```
📦 your-repo-name/
├── 📁 data/
│   ├── 📁 raw/              # Original SLAM 2018 JSON data
│   ├── 📁 interim/          # Parsed & preprocessed pickle files
│   └── 📁 processed/        # Final CSVs with engineered features
│
├── 📁 notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_preprocessing_features.ipynb
│   ├── 03_exploratory_analysis.ipynb
│   ├── 04_ml_baseline_models.ipynb
│   ├── 05_lstm_model.ipynb
│   ├── 06_evaluation_visuals.ipynb
│   └── 07_final_summary.ipynb
│
├── 📁 outputs/
│   ├── 📁 models/           # Trained model pickles
│   └── 📁 eda_visuals/      # Exploratory and final plots
│
├── .gitignore
├── requirements.txt
├── README.md
└── research_proposal.pdf
```

---

### 🧪 Notebooks Overview

| Notebook                    | Description                                                |
| --------------------------- | ---------------------------------------------------------- |
| `01_data_loading`           | Load and inspect parsed session data (`slam_sessions.pk`). |
| `02_preprocessing_features` | Group sessions per user, create behavioral features.       |
| `03_exploratory_analysis`   | Plot feature distributions, detect imbalances.             |
| `04_ml_baseline_models`     | Train Logistic Regression, Random Forest, XGBoost.         |
| `05_lstm_model`             | Build an LSTM for sequence-aware churn prediction.         |
| `06_evaluation_visuals`     | Compare models using ROC, F1, AUC, etc.                    |
| `07_final_summary`          | Final reflections, ethical implications, and key findings. |

---

### ⚖️ Ethical Focus Areas

* **Attention Engineering**: Are we optimizing for meaningful engagement or manipulation?
* **Digital Consent**: Are users truly aware of data use?
* **Surveillance vs Insight**: Where does prediction become intrusion?
* **Bias in Churn Modeling**: Are certain user types unfairly flagged?

---

### 🛠 Tech Stack

* Python 3.10+
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* TensorFlow / PyTorch (for LSTM)
* XGBoost
* JupyterLab / VS Code

---

### 📦 Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Create virtual environment**

   ```bash
   python -m venv .venv
   source .venv/bin/activate   # or .venv\Scripts\activate on Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Place the SLAM dataset**

   * Store raw `.json` files inside `data/raw/`.

---

### 📊 Key Features Extracted

* `avg_time`, `total_time`, `session_count`
* `active_days`, `session_type_counts`, `client_counts`
* Platform-wise churn flags
* Sequence input for LSTM (if enabled)

---

### 🔍 Sample Visualizations

* Session activity by platform
* Churn vs retention ratio
* Time of day vs engagement
* ROC curves per model
* Attention spans across users

---

### 🧩 LSTM Use Case

A deep learning LSTM model was added to learn user session sequences over time. This helps understand how **temporal behaviors influence churn**, and whether early signals are detectable.

---

### 🧭 Project Status

| Phase                  | Status         |
| ---------------------- | -------------- |
| Data Parsing & Loading | ✅ Done         |
| Feature Engineering    | ✅ Done         |
| EDA                    | ✅ Done         |
| Baseline Models        | ✅ Done         |
| LSTM Model             | ⚙️ In Progress |
| Ethical Write-Up       | ⚙️ Drafting    |
| Final Submission       | ⏳ Upcoming     |

---

### 📜 License

This research project is for academic and educational purposes only.
All third-party data remains property of the original creators (SLAM 2018 organizers).

---

### 🙌 Acknowledgements

* SLAM 2018 Dataset Contributors
* Faculty Supervisors and Reviewers
* All open-source library maintainers

