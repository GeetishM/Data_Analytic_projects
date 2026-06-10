<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,12,24&height=200&section=header&text=Supply%20Chain%20Analytics%20🚚&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=38&desc=Optimizing%20Delivery%20and%20Identifying%20Bottlenecks&descAlignY=58&descSize=18&descColor=FFF176"/>

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-4CAF50?style=for-the-badge)](https://choosealicense.com/licenses/mit/)

> *Transforming logistics data into predictive insights for reliable delivery.* 📦

</div>

---

## 📋 Table of Contents

<div align="center">

| | | |
|:---:|:---:|:---:|
| [🎯 About](#-about) | [✨ Key Features](#-key-features) | [🔄 Analysis Pipeline](#-analysis-pipeline) |
| [🛠️ Tech Stack](#%EF%B8%8F-tech-stack) | [📁 Project Structure](#-project-structure) | [🚀 Setup Instructions](#-setup-instructions) |

</div>

---

## 🎯 About

A global e-commerce company manages end-to-end order fulfillment across multiple regions. Recently, they have faced **inconsistent delivery performance**, leading to late deliveries and unpredictable order profitability.

**The Goal:** Analyze delivery operations to identify bottlenecks, uncover the driving factors of late shipments, and build a **predictive Machine Learning model** to assess late delivery risk before an order is even processed.

<div align="center">

| 🎯 Area | 💡 Insight Delivered |
|:---:|:---|
| 🚚 Delivery Bottlenecks | Identifying which shipping modes, regions, and products cause delays |
| ⏰ Time-Series Patterns | Uncovering delay trends by month, day of week, and hour |
| 🤖 Predictive Modeling | Random Forest Classifier to predict `Late_delivery_risk` |
| ⚖️ Class Imbalance | Using SMOTE to balance the dataset for accurate modeling |

</div>

---

## ✨ Key Features

<div align="center">

| Feature | Description |
|:---:|:---|
| 🧹 **Data Cleaning** | Handling missing values, dropping redundant features, and parsing dates |
| 🔍 **Exploratory Data Analysis** | Investigating delay rates across demographics and geography |
| 📈 **Visual Storytelling** | Professional Matplotlib/Seaborn visualizations with a custom color palette |
| 🧮 **Feature Engineering** | Frequency encoding for high-cardinality categorical variables |
| 🤖 **Machine Learning** | Random Forest model trained on SMOTE-balanced data |

</div>

---

## 🔄 Analysis Pipeline

```mermaid
flowchart TD
    A([📂 Raw Dataset\nDataCoSupplyChainDataset.csv]):::input

    subgraph EDA[🔍 Exploratory Data Analysis]
        direction TB
        E1[Clean Data & Parse Dates]:::eda
        E2[Calculate Delay Percentages]:::eda
        E3[Identify Top Bottlenecks by Region]:::eda
        E1 --> E2 --> E3
    end

    subgraph PREP[⚙️ Feature Engineering]
        direction TB
        P1["Select Predictors (X) & Target (y)"]:::process
        P2[Frequency Encoding Categories]:::process
        P3[Train/Test Split]:::process
        P4[SMOTE Balancing]:::process
        P1 --> P2 --> P3 --> P4
    end

    subgraph ML[🤖 Predictive Modeling]
        direction TB
        M1[Train Random Forest]:::ml
        M2[Evaluate Predictions]:::ml
        M3[Accuracy, Precision, Recall]:::ml
        M1 --> M2 --> M3
    end

    OUT([💡 Actionable Logistics Insights]):::output

    A --> EDA --> PREP --> ML --> OUT

    classDef input   fill:#1A237E,color:#fff,stroke:none
    classDef eda     fill:#0D47A1,color:#fff,stroke:none
    classDef process fill:#006064,color:#fff,stroke:none
    classDef ml      fill:#1B5E20,color:#fff,stroke:none
    classDef output  fill:#4A148C,color:#fff,stroke:none
```

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|:---:|:---:|:---|
| 🐍 Language | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Core programming |
| 📓 Notebook | ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white) | Interactive development |
| 🐼 Data | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) | Data manipulation |
| 📉 Viz | ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat) | Statistical data visualization |
| 🤖 ML | ![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white) | Random Forest modeling |
| ⚖️ Imbalance | ![Imbalanced-Learn](https://img.shields.io/badge/Imbalanced_Learn-8A2BE2?style=flat) | SMOTE data balancing |

</div>

---

## 📁 Project Structure

<details>
<summary><b>📂 Click to expand</b></summary>

```
supply_chain_data_analysis/
│
├── 📋 DataCoSupplyChainDataset.csv       # Raw dataset
├── 📓 Supply_Chain_Analysis.ipynb        # Full EDA & ML pipeline
├── 📁 venv/                              # Virtual Environment (Isolated dependencies)
└── 📖 README.md                          # This documentation file
```

</details>

---

## 🚀 Setup Instructions

**1️⃣ Navigate to the project folder**
```bash
cd supply_chain_data_analysis
```

**2️⃣ Activate the Virtual Environment**
*(If you haven't created one, run `python -m venv venv` first)*
```bash
# Windows
.\venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
```

**3️⃣ Install required Python libraries**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

**4️⃣ Launch Jupyter Notebook**
```bash
jupyter notebook
```

> Open `Supply_Chain_Analysis.ipynb` to run the full pipeline and train the model.

---

<div align="center">

⭐ If this project helped you, consider giving it a star!

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,12,24&height=100&section=footer"/>

</div>
