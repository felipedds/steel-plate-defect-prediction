### Goal Project
Predict the probability of various defects on steel plates.

### Evaluation Project
This solution was evaluated using area under the ROC curve using the predicted probabilities and the ground truth targets.
To calculate the final score, AUC is calculated for each of the 7 defect categories and then averaged. In other words, the score is the average of the individual AUC of each predicted column.

##
For each id in the test set, you must predict the probability for each of 7 defect categories: Pastry, Z_Scratch, K_Scatch, Stains, Dirtiness, Bumps, Other_Faults. The file should contain a header and have the following format:
```
id,Pastry,Z_Scratch,K_Scatch,Stains,Dirtiness,Bumps,Other_Faults
19219,0.5,0.5,0.5,0.5,0.5,0.5,0.5
19220,0.5,0.5,0.5,0.5,0.5,0.5,0.5
19221,0.5,0.5,0.5,0.5,0.5,0.5,0.5
etc.
```

#### Competition from Kaggle
Walter Reade, Ashley Chow. (2024). Steel Plate Defect Prediction. Kaggle. `https://kaggle.com/competitions/playground-series-s4e3`

##### Dataset from UCI
`https://archive.ics.uci.edu/dataset/198/steel+plates+faults`