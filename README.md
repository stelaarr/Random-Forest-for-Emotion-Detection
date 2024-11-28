# Random-Forest-for-Emotion-Detection

## Project Details  
- **Objective**: To create a machine learning model for the automatic recognition of human emotions.  
- **Dataset Split**:  
  - **Train/Validation/Test**: 70% / 20% / 10%  

---

## Selected Model  
- **Model Used**: Random Forest Classifier  

---

## Hyperparameter Tuning  
To optimize the performance of the Random Forest model, two methods were employed:  

1. **Grid Search**  
   - **Hyperparameters Tuned**:  
     - Number of trees in the forest: `[91, 117, 130, 172]`  
     - Criterion for quality of split: `["gini", "entropy", "log_loss"]`  
     - Maximum depth of the tree: `[3, 7, 17]`  

2. **Random Search**  
   - **Hyperparameters Tuned**:  
     - Number of trees in the forest: Range from `17` to `237` (step: `20`)  
     - Criterion for quality of split: `["gini", "entropy", "log_loss"]`  
     - Maximum depth of the tree: Range from `3` to `103` (step: `10`)  

---

## Best Hyperparameters  
- **Method Used**: Random Search  
- **Best Parameters**:  
  - **Number of Trees**: `197`  
  - **Maximum Depth**: `33`  
  - **Criterion**: `'entropy'`  

---

## Model Performance  
- **Test Set Accuracy**: **69.23%**  

---

## Notes  
- The Random Forest model was selected for its robustness and effectiveness in handling complex datasets.  
- Random Search yielded the best hyperparameters, outperforming Grid Search in validation accuracy.  
- Further improvements could involve trying additional algorithms or fine-tuning the dataset preprocessing.  

---
