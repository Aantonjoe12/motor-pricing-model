# Motor Insurance Pricing Model (GLM with Tweedie Distribution)

This project builds a full motor insurance pricing model using a Tweedie GLM. It covers everything from preparing the data to modelling, creating the pricing table, visualising the results, and interpreting the final structure.

The goal is to show a clear actuarial workflow for developing a pure premium model and turning the model outputs into a practical pricing structure.

---

## Project Structure

```
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
```



### **01_data_preparation.ipynb**
- Loads and cleans the raw dataset
- Handles missing values and prepares the variables for modelling
- Produces the final dataset used in the GLM  

### **02_exploratory_data_analysis.ipynb**
- Looks at key patterns in the data
- Highlights important rating factors
- Creates the first set of charts

### **03_glm_modelling.ipynb**
- Fits a Tweedie GLM to estimate pure premiums
- Calculates relativities for each factor
- Checks how well the model performs

### **04_pricing_output.ipynb**
- Builds the pricing table from the model results
- Creates bar charts, heatmaps, and comparisons
- Saves all figures for use in later notebooks

### **05_interpretation.ipynb**
- Explains the pricing structure
- Checks that the patterns make sense
- Summarises the main findings 

---
 
## Key Findings

- **Power** and **Region** are the strongest predictors of risk  
- **DriverAge** and **Density** have smaller effects  
- The pricing structure is stable, interpretable, and aligned with actuarial intuition  
- The model provides a solid foundation for building a full pricing engine

## Data Availability

The original dataset used in this project comes from Kaggle:

**Dataset:** [freMTPL - French Motor TPL Insurance Claims Data]  
**Source:** https://www.kaggle.com/datasets/karansarpal/fremtpl-french-motor-tpl-insurance-claims?select=freMTPLsev.csv

The file is not included in this repository because it exceeds GitHub’s file size
limit. To run the notebooks, download the dataset from Kaggle and place it in a
`data/` folder.

## About the Project  
I created this project to practise and demonstrate the full workflow behind a motor insurance pricing model. It covers everything from cleaning the data to fitting the GLM and turning the results into a pricing table.

## Purpose  
The purpose is to show my approach to actuarial modelling, how I think about pricing decisions, and how I communicate technical results in a clear and structured way.
