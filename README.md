# Project Title
Monthly Image base Question and Answering AI Competition

# Project Overview
Multimodal AI is a technology that combines different types of data, such as text and images, to comprehensively handle a wide range of applications. It can convert images into text and generate images based on text, among other uses. It offers high value in terms of service and challenges the development and advancement of multimodal AI models.

# Competition Participation
- Rank
  - public : 12/536
  - private : 11/536

## Tech Stack
- Python
- pandas
- scikit-learn
- XGBoost

## Data Sources
The project uses the following data sources:
- `train.csv`: Training data
- `test.csv`: Test data
- `building_info.csv`: Building information data
- if you want to get datas, please visit (https://dacon.io/competitions/official/236125/overview/description)

## Data Preprocessing
- Load and preprocess training and test data.
- Translate and label encode building information data.
- Handle date and time data and create various time-related features.
- Handle missing values and add interaction features.

## Model Training
- Train XGBoost models with different optimal hyperparameters for each building.
- Optimal hyperparameters for each building are extracted from the `parameters_opt.csv` file.
- Models are trained using XGBoost, aiming to minimize the weighted mean squared error.

## Folder Structure
```
├── data/
│   ├── train.csv
│   ├── test.csv
│   ├── building_info.csv
├── codes/
│   ├── preprocessing.py
│   ├── model_tunning.py
│   ├── inference.py
│   ├── bayesian_optimization.py
├── saved_models/
│   ├── models_version_number/
├── README.md
├── script.py
```

## Script.py
To run the project pipeline, you can use the following command-line options:
```
- `-p` or `--preprocess`: Run data preprocessing.
- `-t` or `--train`: Run model training.
- `-i` or `--inference`: Run model inference.
- `-b` or `--bayesian`: Run Bayesian optimization.
- `proj_name`: Optional project name to be used for saving or loading models.
```
Example usage:
```
python script.py -p -t -i My_Project
```
## Evaluation Metrics
The project uses the following evaluation metrics:
- SMAPE (Symmetric Mean Absolute Percentage Error)
- Weighted Mean Squared Error


