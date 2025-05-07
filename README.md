# molecular-digital-twins
A molecular digital twin simulating LDHA inhibitors in cancer metabolism, combining machine learning and docking to predict compound efficacy, binding, and metabolic impact—accelerating drug discovery with rapid in silico testing.

## Pipeline Overview

1. **Data Preparation**
- Collect LDHA inhibitor data (ChEMBL, BindingDB).
- Clean and preprocess SMILES, IC50, and activity labels.

2. **Molecular Fingerprinting**
- Use RDKit to generate ECFP/Morgan fingerprints.

3. **Machine Learning**
- Train models (RandomForest, XGBoost) to classify active vs inactive compounds.

4. **Molecular Docking**
- Run docking simulations using AutoDock Vina.
- Save binding affinities (`docking_results.csv`).

5. **Digital Twin Simulation**
- Model metabolic responses under LDHA inhibition.
- Analyze how inhibitors reshape cancer cell metabolism.

6. **Visualization**
- Feature importance (SHAP)
- Docking vs bioactivity plots
- 2D/3D compound visualization

## Requirements
numpy
pandas
matplotlib
seaborn
rdkit
xgboost
scikit-learn
shap
py3Dmol

## Install them with:
*!pip install -r requirements.txt*

## Outputs
- IC50 distribution plots  
- Class balance graphs  
- 2D molecular structures  
- Interactive 3D docking visualizations  
- Docking score vs bioactivity scatterplots

## References
- Bader DA, et al. (2020). *Targeting lactate metabolism for cancer therapeutics.* [DOI](https://doi.org/10.xxxx)
- ChEMBL Database: https://www.ebi.ac.uk/chembl/
- AutoDock Vina: https://vina.scripps.edu/
- RDKit: https://www.rdkit.org/

## License
This project is licensed under the MIT License.

## Acknowledgments
Special thanks to the open-source ML and chemistry community and the creators of RDKit, AutoDock Vina, and py3Dmol for making this project possible.
