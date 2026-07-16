# Employee Attrition Prediction — Project

## Overview
This Streamlit app (`app.py`) predicts whether an employee is likely to leave (attrition) using a saved model (`model.pkl`). The app accepts feature values via a form and returns a prediction.

## Data used in `app.py`
The app collects the following features (these correspond to the model input columns):

- Age
- BusinessTravel
- DailyRate
- Department
- DistanceFromHome
- Education
- EducationField
- EmployeeCount
- EmployeeNumber
- EnvironmentSatisfaction
- Gender
- HourlyRate
- JobInvolvement
- JobLevel
- JobRole
- JobSatisfaction
- MaritalStatus
- MonthlyIncome
- MonthlyRate
- NumCompaniesWorked
- Over18
- OverTime
- PercentSalaryHike
- PerformanceRating
- RelationshipSatisfaction
- StandardHours
- StockOptionLevel
- TotalWorkingYears
- TrainingTimesLastYear
- WorkLifeBalance
- YearsAtCompany
- YearsInCurrentRole
- YearsSinceLastPromotion
- YearsWithCurrManager

Notes:
- The feature names and typical value ranges are defined inside `app.py` form fields. The dataset used to train the model appears to be an HR / employee attrition dataset (similar to IBM HR Analytics), but the repository does not contain the original CSV. The trained model file is `model.pkl`.

## Video recording
A recording related to this project was found at:

- [project run/20260716-1143-22.2466684.mp4](project%20run/20260716-1143-22.2466684.mp4)

You can open this video to review a demo or recorded walkthrough. If you want the video embedded or referenced inside the app, tell me where to display it and I can add UI code to `app.py`.

## Requirements and installation
The project includes `requirements.txt`. To set up and run the app locally on Windows, follow these commands.

1. Create a virtual environment (if you don't have one):

```bash
python -m venv .venv
```

2. Activate the virtual environment:

- Command Prompt:

```cmd
.venv\Scripts\activate
```

- PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

3. Install the required Python packages:

```bash
pip install --upgrade pip
pip install -r requirements.txt
pip install streamlit
```

(If you already used the provided `.venv`, packages may already be installed.)

## Run the app
From the project root (after activating `.venv`):

```bash
# preferred (Streamlit runner)
streamlit run app.py

# or run directly with Python
python app.py
```

If you run with `python app.py`, Streamlit will still start the app but using the `streamlit` package.

## Model file
Make sure `model.pkl` is present in the project root. If `app.py` shows the error "Model file 'model.pkl' not found", train and save your model to `model.pkl` or place the provided model there.

## Next steps I can help with
- Embed the demo video into the Streamlit UI.
- Add the original dataset (CSV) and a short data description (source, sample rows).
- Add a small CONTRIBUTING or USAGE section describing expected model output values.

---
Generated automatically from `app.py` and the project files. If you want changes or more details, tell me which parts to expand.