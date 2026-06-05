# 🔍 FraudGT: Graph Transformer for Financial Fraud Detection

## 📌 Overview

**FraudGT** is a simple, effective, and efficient **Graph Transformer-based framework** designed for detecting financial fraud. It leverages graph-based representations of transactional data to capture complex relationships and identify suspicious patterns in financial systems.

This repository contains the complete implementation of the FraudGT framework, including environment setup, dataset configuration, and experiment scripts.

---

## ⚙️ Environment Setup

We recommend using **Conda** to manage dependencies.

### Step 1: Create Environment

```bash
conda create -n fraudGT python=3.9 -y
conda activate fraudGT
```

### Step 2: Install Dependencies

```bash
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
conda install pyg -c pyg
pip install -r requirements.txt
```

---

## 📂 Dataset Setup

1. Download the **Anti-Money Laundering (AML)** dataset
2. Unzip the dataset
3. Place the file (e.g., `HI-small.csv`) inside your dataset directory:

```
./data/HI-small.csv
```

📌 Note: The dataset will be automatically processed during the first run.

---

## ⚙️ Configuration

Before running the model, update the configuration file located at:

```
./configs/{dataset_name}/
```

Example configuration:

```yaml
out_dir: ./results
dataset:
  dir: ./data
```

* `out_dir`: Directory to store results
* `dataset.dir`: Path to dataset

---

## 🚀 Running the Project

A script is provided for easy experimentation.

### Step 1: Navigate to Project Directory

```bash
cd FraudGT
```

### Step 2: Give Execution Permission

```bash
chmod +x ./run/interactive_run.sh
```

### Step 3: Run the Script

```bash
./run/interactive_run.sh
```

---

## 🧪 Experiments

* Easily configurable via YAML files
* Supports different datasets and output directories
* Logs and results are saved in the specified `out_dir`

---

## 📊 Features

* ✔️ Graph Transformer architecture for fraud detection
* ✔️ Efficient handling of financial transaction graphs
* ✔️ Scalable and configurable pipeline
* ✔️ Automated dataset preprocessing

---

## 🎯 Applications

* Financial fraud detection
* Anti-money laundering systems
* Risk analysis in banking networks
* Transaction anomaly detection

---

## 📈 Future Improvements

* Integration with larger real-world datasets
* Model optimization for faster inference
* Visualization of fraud patterns in graphs

---

## 👩‍💻 Author

**Shruti Chauhan**

---

## ⭐ Short Description (for GitHub)

*A Graph Transformer-based framework for efficient and scalable financial fraud detection using transactional graph data.*
