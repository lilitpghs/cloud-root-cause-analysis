# Cloud Application Performance Analysis 

## Overview

This project analyzes distributed application trace data to identify patterns associated with application errors and investigate which microservices may contribute to performance issues. The goal is to turn complex operational data into interpretable insights that can support troubleshooting, prioritization, and data-driven decision-making.

## Business Problem

In complex cloud applications, identifying the components associated with errors can be difficult. This project explores how structured data analysis and explainable models can help technical teams investigate abnormal behavior and prioritize areas for further investigation.

## Key Findings

- **High classification performance:** XGBoost achieved approximately 99% precision and 99% recall for erroneous traces on the test set, demonstrating strong performance in distinguishing erroneous from normal traces.
- **Identification of important components:** Microservices such as `compare-edge-context`, `post-process-ads`, and `user-db.getuserinfostruct` appeared among the influential features across the analyses.
- **Data representation affects results:** Different ways of structuring application traces produced different classification and explanation outcomes.
- **Cross-validation of insights matters:** Comparing rule-based explanations, permutation importance, and SHAP helped assess whether different analytical approaches highlighted similar signals.
- **Operational limitation:** High predictive performance does not prove the actual cause of an error. The identified patterns require validation by application experts.

## Analytical Approach

1. Structured and transformed application trace data into analytical datasets.
2. Compared normal and erroneous traces.
3. Evaluated classification performance across different analytical approaches.
4. Investigated influential features and recurring patterns.
5. Compared explanations and assessed their usefulness and limitations.

## Business Relevance

The analysis demonstrates how operational data can be transformed into actionable investigative leads. Similar approaches can help organizations prioritize troubleshooting efforts, improve monitoring practices, and make complex analytical results more interpretable for technical and business stakeholders.

The study does not quantify reductions in downtime, troubleshooting time or operational costs.

## Dataset

The study analyzed 5,899 application traces:
- **3,145** normal traces
- **2,754** erroneous traces

The original dataset is not publicly available, so the complete workflow cannot be independently reproduced from this repository alone.

## Tools

- Python
- pandas
- scikit-learn
- XGBoost
- SHAP
- t-SNE
- Weka / RIPPER

## Limitations

The findings represent associations rather than verified causal relationships. Results depend on the trace features and analytical methods used, and the original dataset is unavailable for public reproduction.
