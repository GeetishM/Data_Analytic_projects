<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=4,8,24&height=200&section=header&text=Customer%20Trends%20Analysis%20📊&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=38&desc=Uncovering%20Shopping%20Behavior%20with%20Data&descAlignY=58&descSize=18&descColor=FFF176"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=1000&color=FFD54F&center=true&vCenter=true&width=700&lines=4%2C000%2B+Customer+Records+Analyzed+%F0%9F%93%8B;Python+%2B+MySQL+%2B+Power+BI+Pipeline+%F0%9F%94%84;EDA+%7C+Segmentation+%7C+Sales+Trends+%F0%9F%93%88;Actionable+Business+%26+Marketing+Insights+%F0%9F%92%A1)](https://git.io/typing-svg)

<br/>

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![MySQL](https://img.shields.io/badge/MySQL-Data%20Storage-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://mysql.com)
[![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![License](https://img.shields.io/badge/License-MIT-4CAF50?style=for-the-badge)](https://choosealicense.com/licenses/mit/)

> *Turning raw shopping data into decisions that drive business growth* 📊

</div>

---

## 📋 Table of Contents

<div align="center">

| | | |
|:---:|:---:|:---:|
| [🎯 About](#-about) | [✨ Key Features](#-key-features) | [🔄 Analysis Pipeline](#-analysis-pipeline) |
| [🛠️ Tech Stack](#%EF%B8%8F-tech-stack) | [📁 Project Structure](#-project-structure) | [📸 Dashboard Preview](#-dashboard-preview) |
| [🚀 Setup Instructions](#-setup-instructions) | [👤 Author](#-author) | |

</div>

---

## 🎯 About

This project explores **customer shopping behavior** to uncover insights about purchasing patterns, product preferences, and key sales drivers. It aims to help businesses make **data-driven decisions** to enhance:

<div align="center">

| 🎯 Area | 💡 Insight Delivered |
|:---:|:---|
| 📣 Marketing Strategy | Which customer segments respond best to promotions |
| 📦 Inventory Planning | Top-selling products and seasonal demand patterns |
| 😊 Customer Satisfaction | Behavioral trends that drive loyalty and repeat purchases |
| 💰 Revenue Optimization | Key sales drivers and high-value customer identification |

</div>

---

## ✨ Key Features

<div align="center">

| Feature | Description |
|:---:|:---|
| 🧹 **Data Cleaning** | Preprocessing with Pandas & NumPy — null handling, type casting, deduplication |
| 🔍 **EDA** | Sales trends, demographic breakdowns, and purchasing pattern analysis |
| 🗄️ **SQL Querying** | MySQL-powered customer segment deep-dives |
| 📊 **Power BI Dashboard** | Interactive visual storytelling with filters and drill-downs |
| 💡 **Business Insights** | Actionable recommendations for marketing and strategy teams |

</div>

---

## 🔄 Analysis Pipeline

```mermaid
flowchart TD
    A([📂 Raw Dataset\ncustomer_shopping_behavior.csv]):::input

    subgraph PREP[🧹 Data Preparation]
        direction TB
        P1[Load CSV with Pandas]:::process
        P2[Handle Nulls & Duplicates]:::process
        P3[Type Casting & Normalization]:::process
        P4[Feature Engineering]:::process
        P1 --> P2 --> P3 --> P4
    end

    subgraph SQL[🗄️ SQL Analysis]
        direction TB
        S1[Import to MySQL]:::sql
        S2[Segment Queries\nAge · Gender · Category]:::sql
        S3[Aggregations\nRevenue · Frequency · AOV]:::sql
        S1 --> S2 --> S3
    end

    subgraph EDA[🔍 Exploratory Data Analysis]
        direction TB
        E1[Sales Trend Analysis]:::eda
        E2[Demographic Breakdown]:::eda
        E3[Product Preference Mapping]:::eda
        E4[Correlation Analysis]:::eda
        E1 --> E2 --> E3 --> E4
    end

    subgraph VIZ[📊 Visualization]
        direction TB
        V1[Matplotlib & Seaborn Plots]:::viz
        V2[Power BI Dashboard\nInteractive Filters]:::viz
        V1 --> V2
    end

    OUT([💡 Business Insights\n& Recommendations]):::output

    A --> PREP --> SQL & EDA --> VIZ --> OUT

    classDef input   fill:#1A237E,color:#fff,stroke:none
    classDef process fill:#0D47A1,color:#fff,stroke:none
    classDef sql     fill:#006064,color:#fff,stroke:none
    classDef eda     fill:#1B5E20,color:#fff,stroke:none
    classDef viz     fill:#E65100,color:#fff,stroke:none
    classDef output  fill:#4A148C,color:#fff,stroke:none
```

---

## 📈 Insight Areas

```mermaid
flowchart LR
    D([📦 Customer Dataset\n4,000+ Records]):::input

    D --> A[👥 Customer\nSegmentation]:::node
    D --> B[🛍️ Product\nPreferences]:::node
    D --> C[📅 Purchase\nPatterns]:::node
    D --> E[💰 Sales\nDrivers]:::node

    A --> A1([Age · Gender\nLocation Groups]):::insight
    B --> B1([Top Categories\nBrand Affinity]):::insight
    C --> C1([Seasonal Trends\nFrequency Analysis]):::insight
    E --> E1([Revenue Drivers\nHigh-Value Customers]):::insight

    classDef input   fill:#1A237E,color:#fff,stroke:none
    classDef node    fill:#006064,color:#fff,stroke:none
    classDef insight fill:#37474F,color:#fff,stroke:#FFD54F,stroke-dasharray:3
```

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|:---:|:---:|:---|
| 🐍 Language | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Data processing & analysis |
| 📓 Notebook | ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white) | Interactive analysis environment |
| 🗄️ Database | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) | Data storage & SQL querying |
| 📊 Dashboard | ![PowerBI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) | Visual storytelling & reporting |
| 🐼 Data | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white) | Cleaning & transformation |
| 📉 Viz | ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat) ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat) | EDA charts & plots |

</div>

---

## 📁 Project Structure

<details>
<summary><b>📂 Click to expand</b></summary>

```
customer_trends_data_analysis/
│
├── 📋 customer_shopping_behavior.csv     # Raw dataset (4,000+ records)
├── 📓 data_analysis.ipynb                # Jupyter Notebook — full EDA pipeline
├── 📊 customer_trends_dashboard.pbix     # Power BI interactive dashboard
└── 📖 README.md
```

</details>

---

## 📸 Dashboard Preview

<div align="center">

![Dashboard Screenshot](./customer_trends_data_analysis/customer_behavior_dashboard.png)

</div>

---

## 🚀 Setup Instructions

**1️⃣ Clone the repository**
```bash
git clone https://github.com/GeetishM/Data_Analytic_projects
cd Data_Analytic_projects
```

**2️⃣ Navigate to the project folder**
```bash
cd customer_trends_data_analysis
```

**3️⃣ Install required Python libraries**
```bash
pip install pandas numpy matplotlib seaborn mysql-connector-python
```

**4️⃣ Ensure the dataset is present**
```bash
# The file should already be in the folder:
customer_shopping_behavior.csv
```

**5️⃣ Launch Jupyter Notebook**
```bash
jupyter notebook
```

> Then open `data_analysis.ipynb` to run the full analysis pipeline.

**6️⃣ Open the Power BI Dashboard**

Open `customer_trends_dashboard.pbix` in **Power BI Desktop** to explore the interactive dashboard.

---

## 👤 Author

<div align="center">

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/GeetishM">
        <img src="https://github.com/GeetishM.png" width="80" style="border-radius:50%"/><br/>
        <b>Geetish Mahato</b>
      </a>
    </td>
  </tr>
</table>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/geetish-mahato)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GeetishM)

</div>

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](https://choosealicense.com/licenses/mit/) for details.

---

<div align="center">

⭐ If this project helped you, consider giving it a star!

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=4,8,24&height=100&section=footer"/>

</div>
