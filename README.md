# Interstate-Traffic-Weather-Prediction
This repository contains a Jupyter Notebook and a PDF report exploring traffic and weather patterns from the **Metro Interstate Traffic Volume** dataset. It demonstrates data preprocessing, discretization/normalization, and Bayesian Hidden Markov Model (HMM) inference using [Pyro](https://pyro.ai/) and PyTorch.

## 📂 Project Structure
project/
│
├── notebooks/
│ └── traffic_hmm.ipynb # Main Jupyter Notebook
│
├── report/
│ └── traffic_hmm_report.pdf # PDF report summarizing findings
│
├── data/
│ └── Metro_Interstate_Traffic_Volume.csv # Raw dataset (not included here)
│
└── requirements.txt


## ✨ Features

- **Data Cleaning & Preprocessing:** Sorting by timestamp, handling missing values, removing outliers.
- **Feature Engineering:** Normalization with `StandardScaler` and discretization with `KBinsDiscretizer`.
- **Exploratory Visualization:** Histograms and density plots with Seaborn and Matplotlib.
- **Bayesian HMM in Pyro:** 
  - State-dependent emission parameters with Normal/LogNormal priors.
  - Variational inference using `SVI` and `Trace_ELBO`.
  - Visualization of inferred hidden states and ELBO loss curves.

## 📝 Requirements

Install Python 3.9+ and then install dependencies:
pip install -r requirements.txt

🚀 Usage

Clone the repo:

git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO


Install requirements:

pip install -r requirements.txt


Place the dataset (Metro_Interstate_Traffic_Volume.csv) into the data/ folder.

Run the notebook:

jupyter notebook notebooks/traffic_hmm.ipynb

📊 Outputs

Normalized and Discretized Datasets: Previewed within the notebook.

Histogram Visualizations: Feature distributions and binning.

Inferred Hidden States Plot: Visualizes latent state sequence over time.

ELBO Loss Curve: Tracks variational inference convergence.

📑 Report

A PDF summary of methods, analysis, and results is available in report/traffic_hmm_report.pdf.

🖥️ Results

Main findings are summarized in the project-report.pdf
.

Key metrics, charts, or screenshots can be included here for quick reference.

📚 Technologies Used

Python

Jupyter Notebook

< Pandas, NumPy, Matplotlib, Scikit-learn >


🙌 Acknowledgments
< Metro Interstate Traffic Volume dataset >
< UCI CS179 Intro to Graphical Models Course >
