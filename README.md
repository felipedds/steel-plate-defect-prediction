### Intro
This project aims to provide a comprehensive exploratory data analysis (EDA) and a set of simple models (which will not be optimized), but which can give a vague idea of how to choose the best model for the given data set, with the ultimate goal of making decisions. Through this EDA, we will be able to get a deeper understanding of the structure of the data, the values that have a relationship between them and the missing values and pattern or outliers that may affect when performing the modeling or selecting the model we want to use for prediction/recommendation. By performing an EDA, we can identify potential pitfalls and make the decisions and subsequent processing necessary to improve the performance and accuracy of the models. 

### Goal Project
Predict the probability of various defects on steel plates.

### Evaluation Project
This solution was evaluated using area under the ROC curve using the predicted probabilities and the ground truth targets.
To calculate the final score, AUC is calculated for each of the 7 defect categories and then averaged. In other words, the score is the average of the individual AUC of each predicted column.

### Brief Description
For each id in the test set, you must predict the probability for each of 7 defect categories: Pastry, Z_Scratch, K_Scatch, Stains, Dirtiness, Bumps, Other_Faults. The file should contain a header and have the following format:
```
id,Pastry,Z_Scratch,K_Scatch,Stains,Dirtiness,Bumps,Other_Faults
19219,0.5,0.5,0.5,0.5,0.5,0.5,0.5
19220,0.5,0.5,0.5,0.5,0.5,0.5,0.5
19221,0.5,0.5,0.5,0.5,0.5,0.5,0.5
etc.
```

### Variable information

The data set includes 27 independent variables, as follows:
- X_Minimum
- X_Maximum
- Y_Minimum
- Y_Maximum
- Pixel Areas (Pixels_Areas)
- X Perimeter (X_Perimeter)
- Perimeter Y (Y_Perimeter)
- Sum of Luminosity (Sum_of_Luminosity)
- Minimum of Luminosity (Minimum_of_Luminosity)
- Maximum Luminosity (Maximum_of_Luminosity)
- Length of Conveyer (Length_of_Conveyer)
- TypeOfSteel_A300 (TypeOfSteel_A300)
- TypeOfSteel_A400 (TypeOfSteel_A400)
- Steel Plate Thickness (Steel_Plate_Thickness)
- Edge Index (Edges_Index)
- Empty Index (Empty_Index)
- Square Index (Square_Index)
- Outside X Index (Outside_X_Index)
- Edge X Index (Edges_X_Index)
- Edge Y Index (Edges_Y_Index)
- Global Outside Index (Outside_Global_Index)
- Logarithm of Areas (LogOfAreas)
- Logarithmic X Index (Log_X_Index)
- Logarithmic Y Index (Log_Y_Index)
- Orientation Index (Orientation_Index)
- Luminosity Index (Luminosity_Index)
- Sigmoid of Areas (SigmoidOfAreas)

## Project Structure

```
economic-analysis-fred/
├── data/
│   ├── raw/                 # Raw data files
│   ├── processed/           # Processed data files
│   └── external/            # External datasets or data obtained from external sources
├── notebooks/               # Jupyter notebooks for data exploration, and analysis
├── src/                     # Source code
│   ├── data_preprocessing/  # Scripts or modules for data preprocessing
│   ├── feature_engineering/ # Scripts or modules for feature engineering
│   ├── modeling/            # Scripts or modules for modeling (machine learning models)
│   └── evaluation/          # Scripts for model evaluation and performance metrics
├── reports/                 # Reports generated(HTML, PDF) from analysis and modeling
├── models/                  # Saved models or model artifacts
├── environment.yml          # Conda environment file specifying dependencies
├── README.md                # README file describing the project and its components
└── requirements.txt         # Python dependencies file (alternative to environment.yml)
```

#### Competition from Kaggle
Walter Reade, Ashley Chow. (2024). Steel Plate Defect Prediction. Kaggle. `https://kaggle.com/competitions/playground-series-s4e3`

##### Dataset from UCI
`https://archive.ics.uci.edu/dataset/198/steel+plates+faults`