# Flight Price Prediction using AWS

This repository contains a small project for predicting flight ticket prices using machine learning. The notebooks and data are organized to walk through data cleaning, exploratory data analysis (EDA), feature engineering, and model training. The project is prepared to be deployed or further experimented with on AWS.

## Contents

- `data/` - CSV files used by the notebooks
  - `flight_price.csv` - full dataset (source/master)
  - `train.csv`, `val.csv`, `test.csv` - split datasets used by notebooks
- `notebooks/` - analysis and training Jupyter notebooks
  - `data-cleaning.ipynb` - cleaning steps
  - `eda.ipynb` - exploratory data analysis
  - `feature-engineering.ipynb` - feature transformations
  - `model-training.ipynb` - modeling experiments
  - `eda_helper_functions.py` - helper functions used in notebooks

## Quick start (local)

Prerequisites:

- Python 3.8+ (recommended)
- pip

Install minimal dependencies (create a virtual environment first if desired):

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

If there's no `requirements.txt`, install common packages used in the notebooks:

```powershell
pip install pandas numpy matplotlib seaborn scikit-learn jupyterlab
```

Run the notebooks with Jupyter Lab or Notebook:

```powershell
jupyter lab
```

Open and run the notebooks in the `notebooks/` folder.

## Committing and pushing this README to a GitHub repo

I attempted to push this README to the GitHub repository you provided. If the push requires authentication on your machine, follow one of these common approaches:

- Use HTTPS with a personal access token (PAT). When git prompts for credentials, use your username and the PAT as the password.
- Configure SSH keys and push using the SSH URL for the repo.

Example commands to push (run from the repository root):

```powershell
# add a remote named 'ayush' pointing to the target repository
git remote add ayush https://github.com/AyushSVNIT/flight_price_prediction_using_aws.git
git add README.md
git commit -m "Add project README"
# push to the main branch on the target remote
git push ayush main
```

If you prefer pushing to a branch first and creating a PR, replace `main` with `my-readme` (or another branch name) and then create the PR from GitHub.

## Notes

- If you want me to attempt the push from this environment, I can try, but it will likely require authentication that isn't available here. If you provide a repository access method (for example, an SSH deploy key or a temporary PAT) I can push for you; otherwise follow the commands above locally.

