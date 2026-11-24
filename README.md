# Bike Sharing Demand Analysis

## Project Overview

This project investigates the factors influencing bike-sharing demand using the UCI Bike Sharing Dataset from Capital Bikeshare in Washington, D.C. (2011–2012).

Our goal is to understand how weather, time, and user behavior affect bike rental demand, and whether machine learning can predict rental patterns.

### Research Question

**What factors drive bike-sharing demand, and how do these factors differ between registered and casual users?**

## Dataset

**Source:** [UCI Bike Sharing Dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset)

The dataset includes:
- Hourly and daily bike rental counts.
- Weather conditions and temperature.
- Humidity and wind speed.
- Time, weekday, month, and season.
- Registered and casual user rental counts.

Download the dataset and place the original CSV files in `data/raw/`.

Expected files:
- `hour.csv`
- `day.csv`

## Project Structure

```text
data-sci-final-project/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── figures/
├── results/
├── requirements.txt
├── .gitignore
└── README.md
```

## Setup Instructions

### Requirements

- Python 3.13
- Git
- JupyterLab

### Installation

Clone the repository:

```bash
git clone https://github.com/kelfon/data-sci-final-project.git
cd data-sci-final-project
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it:

**Windows:**
```powershell
.venv\Scripts\Activate.ps1
```

**Mac/Linux:**
```bash
source .venv/bin/activate
```

Install project dependencies:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

Register the Jupyter kernel:

```bash
python -m ipykernel install --user --name bike-sharing-project --display-name "Python (Bike Sharing Project)"
```

Launch JupyterLab:

```bash
jupyter lab
```

Select the `Python (Bike Sharing Project)` kernel when opening a notebook.

### Updating Dependencies

If new packages are required, update `requirements.txt`
and notify the other team members.

Run the following to install updated dependencies:

pip install -r requirements.txt

## Analysis Plan

The project is divided into three main areas:

1. **Data Exploration:** Dataset preparation, data quality, and overall rental trends.
2. **Behavioral Analysis:** Registered vs. casual users, weather effects, and seasonal patterns.
3. **Predictive Modeling:** Regression models, model evaluation, and feature importance.

## Team Contributions

| Team Member | Responsibility |
|---|---|
| Kelsey | Data exploration and preparation |
| Bofan | Behavioral analysis and hypothesis testing |
| Zexiu | Predictive modeling and evaluation |

## Collaboration

- Use separate notebooks for each analysis area.
- Keep raw data unchanged.
- Save generated figures in the appropriate `figures/` subfolder.
- Document changes and assumptions.
- Use Git branches and pull requests to integrate work.