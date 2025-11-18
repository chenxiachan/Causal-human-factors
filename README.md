# From 'What-is' to 'What-if' in Human-Factor Analysis

This repository contains the source code and supplementary materials for the paper: **"From 'What-is' to 'What-if' in Human-Factor Analysis: A Post-Occupancy Evaluation Case"**.

In this study, we advocate for distinguishing between descriptive ('what-is') and interventional ('what-if') questions in Post-Occupancy Evaluation (POE). We apply causal discovery algorithms (specifically GES) to uncover the hierarchical causal structure of occupant satisfaction factors, moving beyond traditional correlation-based analysis.
<img width="2066" height="1187" alt="Figure2" src="https://github.com/user-attachments/assets/d65c5c89-6192-4d58-aef8-ee297eefc35f" />

## 📂 Repository Structure

The analysis pipeline is divided into three sequential steps, represented by the Jupyter Notebooks:

* **`0_Data_Preprocessing.ipynb`**
    * **Purpose:** Handles data cleaning and preparation.
    * **Process:** Filters the raw CBE survey data, handles missing values, encodes variables, and selects the relevant features (124 variables) for analysis.
    * **Output:** A cleaned dataset ready for causal discovery algorithms.

* **`1_Analysis.ipynb`**
    * **Purpose:** Performs the core statistical and causal analysis.
    * **Process:**
        * Conducts traditional "What-is" analysis (Correlation, Significance Testing).
        * Runs the Causal Discovery algorithm (Greedy Equivalence Search - GES) to identify the Causal Skeleton.
        * Distinguishes between causally associated and independent variables.
    * **Output:** Statistical summaries and the discovered causal graph structure (DAG).

* **`2_CausalVis.ipynb`**
    * **Purpose:** Visualizes the results.
    * **Process:** Generates the Directed Acyclic Graphs (DAGs) and other figures used in the paper (e.g., the causal hierarchy of satisfaction factors).
    * **Output:** High-quality figures for interpretation and publication.

## 🚀 Getting Started

### Prerequisites

To run the notebooks, you need Python installed along with the following key libraries:

* `pandas`
* `numpy`
* `matplotlib` / `seaborn`
* `statsmodels`


### Usage

1.  **Data Placement:** Place your raw survey data file (e.g., `.csv` or `.xlsx`) in a folder named `data/` (or modify the path in `0_Data_Preprocessing.ipynb`).
2.  **Run sequentially:**
      * Run `0_Data_Preprocessing.ipynb` to generate the processed data.
      * Run `1_Analysis.ipynb` to perform the causal discovery.
      * Run `2_CausalVis.ipynb` to view the causal graphs and results.

## 📊 Data Availability

This study utilizes data from the **Center for the Built Environment (CBE) Occupant Survey**.

  * Due to privacy and licensing agreements, the raw dataset may not be fully shared in this repository.
  * Researchers interested in the CBE dataset should contact the Center for the Built Environment at UC Berkeley directly.


```
