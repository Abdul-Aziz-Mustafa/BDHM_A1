BDMH ASSINGMENT 1



how to use the code
to runt the code 
step1-open the directory containing py file along with testing and training datset
step2-now open the terminal in the same directory 
step3-python3 group_13.py -tr "kaggle_train.csv" -te "kaggle_test.csv"


First we imported all the nessassry libraries such as pandas numpy and skelearn
then from sklearn we imported specific libraries model wise
such as AdaBoostClassfier,Logistic Regression
then we read the user provided arguments on the terminal as our training data
trained the data

we have defined evaluate_model function in which we are using repeatedStratifiedKFold
then it is evaluating the model score using cross_val_score




the stacking function so declared here is an ensemble method  which is used in ml that compbines multiple classification models to improve prediction accuracy.it uses a meta model from the output of the base model and then finally make predictions

then we defined the model_kendall function which basically performs feature selection based on kendalls corelation coeffcient bt input columns and label .

model_ETC function so used in the code try to select the best feature using extra tree classifier algorithm


Model_LinearSVC function is selectionthe best feature using RGE algorithm for which we have imported the nessasary libraries along with


then we have imported the VarianceThreshold library from scikit-learn and defines a function called Model_VarThreshold, which removes all zero-variance features from the input data using the VarianceThreshold method. The resulting columns are returned by the function. The code then applies the Model_ETC function to the training data and y and stores the first element of the output.

then we have done dimensinality reduction using PCA
doing PCA helped us in feature selection and noice reduction
to further try and optimse the accuracy we follwed up using GradientBoostingClassifier
after doing hit and trials using multiple classifiers we ended up with best GradientBoostingClassifier
 we also checked which model is giving the best accuracy for input model by runnning 
 LazyClassifier on our iinput code
then we ran our best model on the testing data to generate the final output csv
final results in output.csv





