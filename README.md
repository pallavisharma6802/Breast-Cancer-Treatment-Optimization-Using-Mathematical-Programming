# Breast Cancer Treatment Optimization

## Overview
This project develops an optimization framework using **Gamspy** to personalize breast cancer treatment strategies.  
The goal is to balance **maximizing patient survival time** and **minimizing relapse risk** using clinical profiles from the **METABRIC dataset**.

## Key Features
- **Multi-Objective Optimization**: Formulates treatment intensity decisions based on tumor characteristics, patient risk profiles, and cohort constraints.
- **Risk Classification**: Categorizes patients into high-risk and low-risk groups based on tumor size, prognosis index, and relapse-free intervals.
- **Cohort-Based Constraints**: Tailors aggressive vs conservative treatments according to biological subtypes (e.g., LumA, Her2, Basal).
- **Sensitivity Analysis**: Evaluates trade-offs by varying objective function weights.
- **Survival Analysis**: Visualizes outcomes using Kaplan-Meier curves and Pareto efficiency plots.

## Tech Stack
- **Languages**: Python
- **Libraries/Frameworks**: Gamspy, Pandas, Scikit-Learn, Matplotlib, Seaborn
- **Optimization Solver**: CPLEX (via Gamspy interface)

## Dataset
- **METABRIC (Molecular Taxonomy of Breast Cancer International Consortium)** clinical dataset  
  - 2,509 patients
  - Features include survival time, relapse status, tumor size, mutation count, receptor statuses (ER, PR, HER2), and treatment history.


## How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install gamspy pandas matplotlib scikit-learn seaborn
   ```
3. Run the Jupyter notebooks in the `notebooks/` directory sequentially:
   - `data_analysis.ipynb`
   - `optimization_model.ipynb`

## Results
- Identified personalized treatment plans balancing survival and relapse objectives.
- Demonstrated up to **14% improvement** in survival optimization through sensitivity analysis.
- Highlighted survival trends using Kaplan-Meier curves comparing aggressive vs conservative treatments.
