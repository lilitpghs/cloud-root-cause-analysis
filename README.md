
# Cloud Application Root Cause Analysis

## Overview
This project investigates application trace data to identify patterns associated with errors, compare analytical approaches and interpret the factors influencing model predictions. The findings can support root cause investigation, although the identified patterns are not independently verified as actual causes.

## Objectives
- Structure application trace data for analysis.
- Compare approaches for distinguishing normal and erroneous traces.
- Examine influential features and model explanations.
- Interpret findings while recognising the limitations of the analysis.

## Dataset
The original application-trace dataset and intermediate files are not publicly available. Therefore, the full analysis cannot be reproduced from this repository alone.

## Notebook
Open `cloud_analytics.ipynb` to explore the analytical workflow and any saved visual outputs.

## Tools
Python, pandas, scikit-learn, XGBoost, SHAP and data visualisation.

## Limitations
The analysis identifies patterns associated with traces labelled as erroneous. These patterns and model explanations do not, by themselves, establish the actual operational root cause.
