====================== OVERVIEW ======================

All preprocessing, modelling and testing steps are completely reproducable, as all necessary data is contained in this folder.

'A_Preprocessing.ipynb' computes all preprocessing steps and saves final train/test data.
    > Input: 'strokedata.csv'
    > Output: 'train.csv', 'test.csv', 'X_train_SMOTE.csv', 'y_train_SMOTE.csv'

'B_Modelling.mlx' Main script: Training, tuning, and testing of all models. Saves best models.
    > Input: 'train.csv', 'test.csv', 'X_train_SMOTE.csv', 'y_train_SMOTE.csv'
    > Output: 'dt_best.mat', 'knn_best.mat'

'C_Test_Final_Model.mlx' loads best models and tests them on the test data.
    > Input: 'test.csv', 'dt_best.mat', 'knn_best.mat'
    > Ouput: None


================ TESTING INSTRUCTIONS =================

To test the best model, simply run 'C_Test_Final_Model.mlx'.


==================== DEPENDENCIES ===================== 

'MATLAB' version 9.11

'Statistics and Machine Learning Toolbox' version 12.2

All code was written in MATLAB R2021b.