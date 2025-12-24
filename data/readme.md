# Data Requirements

This project utilizes the dataset from the **ESA Kelvins Collision Avoidance Challenge**. 

## How to get the data
Due to file size limitations on GitHub, the raw CSV files are not included in this repository. You can download the dataset directly from the official competition platform:

* **Source:** [ESA Kelvins - Collision Avoidance Challenge](https://kelvins.esa.int/collision-avoidance-challenge/data/)
* **Files needed:** `train_data.csv` (and `test_data.csv` if applicable)

## Setup Instructions
1. Download the `train_data.csv` file from the link above.
2. Place the file inside this `/data` directory.
3. Ensure the filename matches exactly as `train_data.csv` for the notebooks to run correctly.

## About the Data
The dataset consists of **Conjunction Data Messages (CDMs)** containing over 100 features related to satellite orbital mechanics and space weather, including:
- **Orbital State:** Position ($r, t, n$) and velocity vectors.
- **Uncertainty:** Covariance matrices for both primary and secondary objects.
- **Space Weather:** Solar Radio Flux (F10.7), Sunspot Number (SSN), and Geomagnetic Index (AP).
- **Target Variable:** The `risk` (probability of collision).



---
*Note: This data is provided by the European Space Agency for research and competition purposes.*