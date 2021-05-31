# Approach

* EDA is performed and Understood about Imbalance of dataset and outlier features

* Used SMOTE to treat imbalance in dataset and used clipping to treat outliers

* Used Dummy encoding for categorical features and Used Standard Scaler for scaling numerical features

* Aggregation of features using automtic feature selection tool to improve model

* Started with Vanila SVM, Logistic and KNN Classifiers which performed on the lower side.

* CATboost are selected and hypertuned to optimize the roc_auc score as data is mostly categorical

* Used XGBoost, Random Forest and LightGBM hypertuned to optimize the score but the performance is similar to CATboost

* All three CATBoost, XGBoost, LightGBM and Random Forest showed similar Train and Validation Scores 

* This Indicated the the model is not verfitting but suffering from bias.

* Tried Oversampling, Undersampling the data to check if imbalance in data is the cause. But Performance didnt have significant affect

* Tried an ensemble method by Averging all four models the model performnce didn't improve much

* Tried to combine features using Automtic Feature generator and trained the model on Neural Nets but there was no significant affect

* XGBoost seems to have high ROC_AUC on both validation and test set

* XGBoost is selected as final model for predicting on Test Set

