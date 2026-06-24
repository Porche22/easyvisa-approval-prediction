# EasyVisa — Visa Approval Prediction

> **Category:** Machine Learning &nbsp;·&nbsp; **Type:** Jupyter notebook project

## Overview

# EasyVisa: Predicting Visa Application Status

## 1\. Problem Definition and Objective

**Context:** Business communities in the United States are facing high demand for human resources but struggle with the challenge of identifying and attracting the right talent, both locally and from abroad. The Immigration and Nationality Act (INA) allows US employers to hire foreign workers on a temporary or permanent basis, a process overseen by the Office of Foreign Labor Certification (OFLC). The OFLC processes job certification applications, granting them when employers can demonstrate that no sufficient US workers are available for the role at a fair wage.

**Problem:** The number of visa applications is increasing significantly each year, making the manual review of every case a tedious and time-consuming task for the OFLC. The firm "EasyVisa" has been hired to provide a data-driven solution to this problem.

**Objective:** The primary goal of this project is to build a classification model that can help EasyVisa in the following ways:

  1. **Facilitate the process of visa approvals:** By accurately predicting the outcome of a visa application (Certified or Denied).
  2. **Recommend a suitable profile for applicants:** By identifying the key drivers and factors that significantly influence the visa certification status. This will help employers understand what constitutes a strong application.

## 2\. Data Dictionary

The dataset contains various attributes of the employee and the employer.

Feature | Description | Data Type  
---|---|---  
`case_id` | Unique ID of each visa application | Character  
`continent` | Continent of the employee's origin | Character  
`education_of_employee` | Education level of the employee | Character  
`has_job_experience` | Does the employee have any job experience? (Y/N) | Character  
`requires_job_training` | Does the employee require any job training? (Y/N) | Character  
`no_of_employees` | Number of employees in the employer's company | Integer  
`yr_of_estab` | Year in which the company was established | Integer  
`region_of_employment` | The region of the employer's intended work location | Character  
`prevailing_wage` | The prevailing wage for the job in the intended area | Float  
`unit_of_wage` | The unit of the prevailing wage (Hour, Week, Month, Year) | Character  
`full_time_position` | Is the position full-time? (Y/N) | Character  
`case_status` | **Target Variable:** Visa application status (Certified/Denied) | Character

## Project deep dive

This repository contains a complete, end-to-end notebook for **EasyVisa**.
It walks through the full workflow — from framing the problem and exploring the
data, through modeling and evaluation, to the conclusions and recommendations.

- **24 code steps** of analysis and modeling
- Full outputs, tables, and visualizations preserved in the rendered HTML
- A runnable `notebook.ipynb` so you can re-execute and extend the work

## Tech stack

`google-generativeai`, `imbalanced-learn`, `matplotlib`, `numpy`, `pandas`, `scikit-learn`, `seaborn`, `shap`, `xgboost`

## What's in this repo

| File | Description |
|------|-------------|
| [`notebook.ipynb`](notebook.ipynb) | The runnable notebook (code recovered from the original export) |
| [`easyvisa-approval-prediction.html`](easyvisa-approval-prediction.html) | Full rendered notebook with **all outputs & plots** preserved |
| `requirements.txt` | Python dependencies inferred from the notebook |

## View the notebook

GitHub renders `.ipynb` files inline — just open [`notebook.ipynb`](notebook.ipynb).
For the fully-rendered version with every saved output and figure:

- **Rendered notebook (nbviewer):** https://nbviewer.org/github/Porche22/easyvisa-approval-prediction/blob/main/notebook.ipynb
- **Rendered HTML export:** https://htmlpreview.github.io/?https://github.com/Porche22/easyvisa-approval-prediction/blob/main/easyvisa-approval-prediction.html

> Replace `Porche22` with your GitHub username after pushing.

## Run it locally

```bash
git clone https://github.com/Porche22/easyvisa-approval-prediction.git
cd easyvisa-approval-prediction
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook notebook.ipynb
```

---

<sub>Notebook reconstructed from an nbconvert HTML export; code cells recovered
faithfully, rich outputs are preserved in the accompanying `.html`.</sub>
