# PROTEIN-STRUCTURE-MODELLING-SWISS-MODELLING-2QAC-closed-MTIP-MyosinA-tail-complex
PROTEIN-STRUCTURE-MODELLING [SWISS MODELLING] = 2QAC = The closed MTIP-MyosinA-tail complex from the malaria parasite invasion machinery
# Comparative Protein Structure Modeling: Myosin A Tail Domain Interacting Protein (MTIP) 🧬🔬

## Overview

This repository contains the prediction results from two major computational tools, **SWISS-MODEL** (Homology Modeling) and **I-TASSER** (Threading/Hybrid Modeling), for the **Myosin A tail domain interacting protein (MTIP)**. MTIP is a crucial component of the parasite invasion machinery (glideosome), making its accurate structure important for drug design against parasites like *Plasmodium falciparum*.

The goal of this project was to generate and compare high-confidence 3D models of the MTIP protein.

---

## Target System and Methodology

* **Target Protein:** Myosin A tail domain interacting protein (MTIP).
* **Target Sequence ID:** `2QAC mutated.fasta`.
* **Primary Predicted Oligo-State (SWISS-MODEL):** Monomer (based on the input sequence, though the template suggests a hetero-dimer/trimer complex).
* **Modeling Tools:** **SWISS-MODEL** and **I-TASSER**.

### Key Model Quality Metrics (SWISS-MODEL)

The high sequence identity (over 99% with known MTIP structures) confirms the homology model is of extremely high quality.

| Metric | SWISS-MODEL Value | Interpretation |
| :--- | :--- | :--- |
| **Template Identity** | **99.31%** | Excellent match with templates like PDB ID 2qac. |
| **Global Model Quality Estimate (GMQE)** | **0.91** | High score, indicating a reliable overall fold. |
| **QMEANDisCo Global** | $\mathbf{0.85 \pm 0.07}$ | Quality score comparable to high-resolution experimental structures. |
| **I-TASSER C-score** | [Check I-TASSER results and insert C-score] | Measures confidence of I-TASSER models (C-score $\in [-5, 2]$, higher is better). |

---

## Repository Files

The files are organized to support the structural analysis and comparison of the two prediction methods.

### 🔬 Structural Outputs and Core Reports

| File Name | Description | Source |
| :--- | :--- | :--- |
| **model\_01.pdb** | **The final predicted 3D structure** of the MTIP protein (from SWISS-MODEL). | SWISS-MODEL |
| `report.html` | Full interactive SWISS-MODEL report, including all visualization charts and metrics. | SWISS-MODEL |
| `I-TASSER results.pdf` | **Full report from I-TASSER**, detailing predicted models (C-scores, TM-scores), and functional annotation. | I-TASSER |
| `2QAC mutated.fasta _ Summary.pdf` | Summary of the SWISS-MODEL run (templates, sequence identity). | SWISS-MODEL |
| `Original 2qac & 2aqc mutated alignmet.psw` | Raw alignment file used during preparation (likely for ProMod3/SWISS-MODEL). | Input/Context |

### 📈 Quality Visualizations

| File Name | Purpose |
| :--- | :--- |
| `Local_quality_estimate.png` | Graphical plot of the residue-by-residue local quality score (QMEANDisCo). | SWISS-MODEL |
| `Quality_comparison.png` | Graph comparing the model's overall quality (QMEAN) against the distribution of solved experimental structures. | SWISS-MODEL |

---

## Setup and Usage

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    cd [Your Repository Name]
    ```

2.  **View 3D Structure:**
    Load the **`model_01.pdb`** file into any molecular visualization software (e.g., **PyMOL**, **ChimeraX**, or **VMD**) to inspect the predicted MTIP structure.

3.  **Analyze Reports:**
    * Open **`report.html`** in a web browser for detailed, interactive homology modeling results.
    * Review **`I-TASSER results.pdf`** to evaluate the top models predicted by the threading method and compare their confidence (C-score) and functional predictions.
