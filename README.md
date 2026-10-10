# Task 3 — Customer Churn Prediction

This project predicts whether a customer is likely to leave (`Exited = 1`) or stay (`Exited = 0`) using the supplied Churn Modelling dataset.

## Project contents

```text
customer_churn_prediction_project/
├── customer_churn_prediction.ipynb
├── data/
│   └── Churn_Modelling.csv
├── results/       # Metrics and plots are generated here
├── artifacts/     # Trained model is generated here
├── requirements.txt
└── README.md
```

## Setup

Python 3.10–3.12 is recommended.

```bash
python -m venv .venv
```

Activate the environment:

- Windows PowerShell: `.venv\Scripts\Activate.ps1`
- macOS/Linux: `source .venv/bin/activate`

Install packages:

```bash
pip install -r requirements.txt
```

## Run

Open `customer_churn_prediction.ipynb` in VS Code or Jupyter Notebook and run cells from top to bottom.

The notebook defaults to `Churn_Modelling.csv` in the current working directory. If the notebook is run from the project root, change the `DATA_PATH` cell to:

```python
DATA_PATH = Path("data/Churn_Modelling.csv")
```

Alternatively, copy `Churn_Modelling.csv` beside the notebook.

## Models and evaluation

- Logistic Regression
- Random Forest
- Gradient Boosting
- Accuracy, precision, recall, F1-score, ROC-AUC and average precision
- Confusion matrices and ROC / precision-recall curves

Outputs are saved to `results/`; the selected model is saved to `artifacts/`.

## Target

`Exited = 1` means the customer exited (churned); `Exited = 0` means the customer stayed.

## Notes

Model scores are generated when you execute the notebook. They are not prefilled or fabricated. This is an educational baseline and should be validated on current business data before production use.
