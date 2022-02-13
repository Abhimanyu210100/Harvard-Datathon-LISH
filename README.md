# Harvard-Datathon-LISH
The repo contains the final code that was used in Harvard Datathon@LISH 2022 to secure 1st place

The jupyter notebook consists of the code for data cleaning and model building that was used for the datathon. 

## Data Cleaning:
- Features were extracted from the date on which the readings were recorded (day, month, year)
- A new feature was created that represented the number of years since the waterpoint has been functional
- The missing data in categorical variables were encoded as a separate category

## Model Details:
- Model created consisted of an ensemble of 10 CATBoost classifiers
- Each classifier was trained on a subset of the dataset and used to create predictions
- This was done to avoid different models from giving the same result (avoiding unnecessary bias in the model)
- Learning rate and depth of the trees were optimised by hyperparameter tunning
