# Motor Insurance Pricing Model (GLM with Tweedie Distribution)

This project builds an end‑to‑end motor insurance pricing model using a Tweedie
Generalised Linear Model (GLM). It includes data preparation, modelling,
pricing table generation, visualisation, and interpretation of results.

The aim is to demonstrate a clear, actuarial‑style workflow for developing a
pure premium model and converting model outputs into a pricing structure.

---

## Project Structure
notebooks/  
01_data_preparation.ipynb
02_eda.ipynb
03_glm_modelling.ipynb
04_pricing_output.ipynb
05_interpretation.ipynb 
data/  
(not included due to size)  
figures/  
bar_chart_power.png  
heatmap.png  
region_chart.png  
README.md  


### **01_data_preparation.ipynb**
- Loads and cleans the raw dataset  
- Handles missing values and variable transformations  
- Prepares the final modelling dataset  

### **02_exploratory_data_analysis.ipynb**
- Explores distributions and relationships  
- Identifies key rating factors  
- Produces initial visualisations  

### **03_glm_modelling.ipynb**
- Fits a Tweedie GLM for pure premium  
- Generates relativities for each factor  
- Evaluates model fit and diagnostics  

### **04_pricing_output.ipynb**
- Builds the pricing table using model relativities  
- Creates bar charts, heatmaps, and factor comparisons  
- Saves figures for later use  

### **05_interpretation.ipynb**
- Interprets the pricing structure  
- Checks monotonicity and reasonability  
- Summarises key findings and next steps  

---
 
## Key Findings

- **Power** and **Region** are the strongest predictors of risk  
- **DriverAge** and **Density** have smaller but logical effects  
- The pricing structure is stable, interpretable, and aligned with actuarial intuition  
- The model provides a solid foundation for building a full pricing engine

## Data Availability

The original dataset used in this project comes from Kaggle:

**Dataset:** [freMTPL - French Motor TPL Insurance Claims Data]  
**Source:** [https://www.kaggle.com/your-dataset-link](https://www.kaggle.com/datasets/karansarpal/fremtpl-french-motor-tpl-insurance-claims?select=freMTPLsev.csv)

The file is not included in this repository because it exceeds GitHub’s file size
limit. To run the notebooks, download the dataset from Kaggle and place it in the
`data/` folder.


