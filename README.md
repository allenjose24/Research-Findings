# Capstone Project: Security Information and Event Management (SIEM) Analysis

This repository contains the research and development files for a capstone project focused on Security Information and Event Management (SIEM). The project involves the analysis of research papers, log data, and the development of a prototype for anomaly detection.

## 📋 Table of Contents

- [About The Project](#about-the-project)
- [Repository Structure](#repository-structure)
- [Research Papers](#research-papers)
- [Team's Understanding](#teams-understanding)
- [Log Data](#log-data)
- [Prototype Notebook](#prototype-notebook)
- [Getting Started](#getting-started)
- [How To Use](#how-to-use)
- [Contributors](#contributors)
- [Acknowledgments](#acknowledgments)

## 🔍 About The Project

This project aims to provide a comprehensive analysis of SIEM systems, their operational roles, challenges, and future trends. The repository includes a collection of research papers that delve into various aspects of SIEM, along with log data from different operating systems and a prototype notebook for anomaly detection using machine learning.

## 📁 Repository Structure

```
Research-Findings/
│
├── README.md                           # Project documentation
│
├── papers/                            # Research papers collection
│   ├── snp14.pdf                     # Operational Role of SIEM Systems
│   ├── C&D_SIEM.pdf                  # Challenges and Directions in SIEM
│   ├── SIEM_Pattern.pdf              # SIEM Architectural Pattern
│   └── SIEM_A,T,U-I.pdf             # SIEM Analysis, Trends, and Usage
│
├── Research Findings.docx         # Team's collaborative analysis
│
├── data/                              # Log data for analysis
│   ├── Mac_2k.log_structured.csv     # macOS log data
│   └── Windows_2k.log_structured.csv # Windows log data
│
└──prototype/
    └── Prototype-001.ipynb           # Anomaly detection prototype

```

## 📚 Research Papers

This repository contains four key research papers that provide a foundational understanding of SIEM systems:

### 1. **"The Operational Role of Security Information and Event Management Systems"** (`snp14.pdf`)
This paper discusses the operational role of SIEM systems within a Security Operations Center (SOC), their architecture, and the challenges they face.

### 2. **"Challenges and Directions in Security Information and Event Management (SIEM)"** (`C&D_SIEM.pdf`)
This paper explores the challenges of integrating SIEM in a real-world Air Traffic Control (ATC) system, particularly with unstructured logs, and proposes solutions using behavioral baselines.

### 3. **"A Security Information and Event Management Pattern"** (`SIEM_Pattern.pdf`)
This paper proposes a generic architectural pattern for SIEM systems to standardize their design and improve modularity and reusability.

### 4. **"Security Information and Event Management (SIEM): Analysis, Trends, and Usage in Critical Infrastructures"** (`SIEM_A,T,U-I.pdf`)
This paper analyzes the trends and usage of SIEM systems in critical infrastructures, their evolution, and future enhancements.

## 📝 Team's Understanding

The `Research Findings.docx` file contains a detailed summary and understanding of the research papers from all team members. It serves as a collaborative knowledge base for the project, providing insights and analysis from multiple perspectives.

## 📊 Log Data

The repository includes two CSV files with structured log data:

- **`Mac_2k.log_structured.csv`**: Contains log data from a macOS environment
- **`Windows_2k.log_structured.csv`**: Contains log data from a Windows environment

This data is used for the analysis and development of the prototype, providing real-world examples of system logs for anomaly detection testing.

## 📓 Prototype Notebook

The **`Prototype-001.ipynb`** Colab notebook contains the implementation of the first prototype for anomaly detection in log data. The notebook uses **Latent Dirichlet Allocation (LDA)** to model behavioral baselines from the log data and identify potential threats.

### Key Features:
- Behavioral baseline modeling
- Anomaly detection using machine learning
- Log data preprocessing and analysis
- Visualization of detected anomalies

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook or Google Colab
- Git

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/allenjose24/Research-Findings.git
   cd Research-Findings
   ```

2. **Install required packages:**
   ```bash
   pip install -r config/requirements.txt
   ```

   If `requirements.txt` doesn't exist, install the following packages:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter gensim nltk
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

## 🔧 How To Use

1. **Review Research Papers:**
   - Navigate to the `papers/` directory
   - Read through the four research papers to understand SIEM fundamentals

2. **Explore Team Findings:**
   - Open `Research Findings.docx` in the `documentation/` folder
   - Review the collaborative analysis and insights

3. **Analyze Log Data:**
   - Examine the CSV files in the `data/` directory
   - Use pandas to load and explore the structured log data:
     ```python
     import pandas as pd
     mac_logs = pd.read_csv('data/Mac_2k.log_structured.csv')
     windows_logs = pd.read_csv('data/Windows_2k.log_structured.csv')
     ```

4. **Run the Prototype:**
   - Open `notebooks/Prototype-001.ipynb` in Jupyter Notebook or Google Colab
   - Follow the notebook cells to understand the anomaly detection implementation
   - Experiment with different parameters and datasets

5. **Extend the Analysis:**
   - Modify the prototype to test different machine learning approaches
   - Add new log data sources for analysis
   - Implement additional visualization techniques

## 👥 Contributors

- **Allen Jose** 
- **Satish Pakalapati** 
- **Nikhil Reddie** 
- **Prem Swaroop**
- **Chankapure Kameshwar**
- **Abijith Chowdary**

## 🙏 Acknowledgments

This project was developed as part of a capstone course and is based on the research and findings from the following papers:

- "The Operational Role of Security Information and Event Management Systems"
- "Challenges and Directions in Security Information and Event Management (SIEM)"
- "A Security Information and Event Management Pattern"  
- "Security Information and Event Management (SIEM): Analysis, Trends, and Usage in Critical Infrastructures"

Special thanks to the academic community for providing comprehensive research on SIEM systems and their applications in cybersecurity.

---

## 📄 License

This project is for educational purposes as part of a capstone course. Please refer to individual research papers for their respective licensing and citation requirements.

## 📞 Contact

For questions or collaboration opportunities, please reach out to the project contributors through their GitHub profiles.

