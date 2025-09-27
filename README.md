# Strategic Sourcing Optimization

This project demonstrates how **data analytics and optimization** can improve procurement and supplier selection. Using synthetic datasets, we simulate a sourcing environment where companies must balance **cost, reliability, lead time, and sustainability** when choosing suppliers.

---

## 📌 Project Summary

- **Objective**: Optimize supplier allocation to **minimize procurement costs** while meeting material demand and respecting supplier constraints.  
- **Key Features**:  
  - Supplier scoring model (cost, reliability, sustainability).  
  - Linear Programming optimization using **PuLP**.  
  - Visualization of supplier allocations.  
- **Outcome**: A data-driven approach to select suppliers and optimize sourcing strategies.

---

## 📊 Dataset

The project uses three synthetic datasets (stored in `/data`):

1. **suppliers.csv**  
   Supplier details including country, lead time, reliability, and sustainability score.  

2. **costs.csv**  
   Cost and capacity constraints per supplier and material.  

3. **demand.csv**  
   Monthly demand for each material.  

---

## ⚙️ Methodology

1. **Data Exploration**  
   - Summarized supplier characteristics.  
   - Compared unit costs vs. supplier performance.  

2. **Supplier Scoring**  
   - Composite score = `0.5*Reliability + 0.3*Sustainability + 0.2*Cost efficiency`.  

3. **Optimization Model (Linear Programming)**  
   - Decision variables: quantity ordered from each supplier.  
   - Objective: minimize total cost.  
   - Constraints:  
     - Supplier max capacity respected.  
     - Total demand for each material satisfied.  

4. **Results & Visualization**  
   - Optimal allocation of materials across suppliers.  
   - Bar charts showing total allocation per supplier.  

---

## 🛠️ Tech Stack

- Python  
- Libraries: `pandas`, `numpy`, `matplotlib`, `pulp`  

---

## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/yourusername/strategic-sourcing-optimization.git
cd strategic-sourcing-optimization

# Install dependencies
pip install pandas numpy matplotlib pulp jupyter

# Run notebook
jupyter notebook strategic_sourcing.ipynb
