# 🧪 Bioreactor Operations & Data Science Test

Welcome! This test is designed to evaluate your ability to work with real-world industrial data for hydrogen-generating bioreactors. The focus is on:

- Data parsing and cleaning  
- Predictive modeling for efficiency or failure  
- System thinking for automation  
- Communication of your process and design

---

## 📦 Files Provided

- `data/`: Raw sensor logs, annotations, and metadata  
- `scripts/data_parser.py`: Write code to clean and merge sensor data  
- `notebooks/modeling_task.ipynb`: Your main modeling notebook  
- `scripts/system_design_diagram.png`: Upload your system architecture here  

---

## 🧭 Tasks

### 1. Domain Understanding (Writeup)

**Deliver in your modeling notebook or as a separate markdown file.**

- Propose 2–3 ML use-cases for improving bioreactor operations  
- Describe key preprocessing steps for modeling time-series sensor data  

### 2. Parsing Task

In `scripts/data_parser.py`, write code to:  
- Read and clean all raw sensor logs  
- Handle missing or corrupted timestamps  
- Merge on a common time index (e.g., 1-minute intervals)  
- Save output to a single `cleaned_data.parquet` file with:  
timestamp | temperature | pressure | flow_rate | pH | DO | voltage | current | H2 | CO2 | CH4 | is_failure

markdown
Copy
Edit

### 3. Modeling Task

In `notebooks/modeling_task.ipynb`, build a model to:  
- Predict drops in `H2_output_efficiency` 60 minutes in advance  
- Use appropriate lagged features, moving averages, etc.  
- Include plots and metrics (RMSE, AUC, or confusion matrix)  
- Explain your model’s behavior and key features  

### 4. System Design

- Create a system architecture to:
- Ingest logs from multiple bioreactors (S3, FTP, or local)
- Parse & validate data  
- Store clean time-series datasets  
- Train models weekly and serve predictions via API  
- Upload a PNG of the diagram in `scripts/system_design_diagram.png`  
- Add a write-up in markdown or in `system_architecture.md`  

---

## ✅ Submission

Please return:
- Your updated `scripts/`, `notebooks/`, and diagram files  
- Clean and modular code  
- README-style documentation if needed  

**Optional but appreciated**: Include a short video walkthrough or demo of your code.

Good luck!
