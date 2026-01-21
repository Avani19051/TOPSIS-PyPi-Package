# TOPSIS-Py (CLI-Based Python Package)

TOPSIS-Py is a **command-line Python package** that implements the  
**TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method,  
commonly used for **Multi-Criteria Decision Making (MCDM)** problems.

This project focuses on **correct theoretical implementation**, **clean workflow**,  
and **ease of use**, making it suitable for **academic projects and practical use**.

---

## ✨ Key Features

| Aspect | Details |
|------|--------|
| Methodology | Classical TOPSIS algorithm |
| Interface | Command-Line Interface (CLI) |
| Input Format | CSV-based decision matrix |
| Validation | Input and argument validation |
| Output | Ranked alternatives with TOPSIS scores |
| Design Goal | Simple, readable, and PyPI-ready |

---

## 📖 About TOPSIS

**TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** is a popular  
decision-making technique used when multiple alternatives must be evaluated  
across several criteria.

### 🔍 Fundamental Concept

An alternative is considered better if it:
- Lies **closest to the ideal (best) solution**
- Lies **farthest from the negative (worst) solution**

This balance helps in generating a rational and interpretable ranking.

---

## 🏭 Areas of Application

| Field | Use Case |
|-----|---------|
| Engineering | Design and material selection |
| Management | Vendor or supplier evaluation |
| Finance | Ranking investment options |
| Data Analytics | Comparing models or strategies |

---
## TOPSIS Algorithm Flow

```mermaid
flowchart TD
    A[Decision Matrix] --> B[Normalization]
    B --> C[Apply Weights]
    C --> D[Determine Ideal Best]
    C --> E[Determine Ideal Worst]
    D --> F[Distance from Ideal Best]
    E --> G[Distance from Ideal Worst]
    F --> H[TOPSIS Score Calculation]
    G --> H
    H --> I[Final Ranking]

## 🧠 Program Workflow

```mermaid
flowchart LR
    A[CLI Arguments] --> B[Input Validation]
    B --> C[Load CSV File]
    C --> D[TOPSIS Computation]
    D --> E[Score & Rank Calculation]
    E --> F[Write Output CSV]
```

---

## 📦 Installation

```bash
pip install topsis-swastik-102303585
```

---

## 🚀 Usage

```bash
python topsis.py <input_file> <weights> <impacts> <output_file>
```

Example:

```bash
python topsis.py data.csv "1,2,1,1" "+,+,-,+" result.csv
```

---

## ⚠️ Limitations

- Categorical data not supported  
- Missing values not allowed  
- Weights must be positive  
- Impacts must be '+' or '-'  

---

## 📜 License

MIT License

