# Medical-Cost-Personal-Datasets-project
a data sceince project (a Regression) over Medical Cost Personal Datasets . the idea is to understand this data set and make it ready to build a model from it 
to predict the charges of new clients
it contain all sort of part like EDA , data preprocessing , model hyperparameter tuning and testing the model
### about datasets
down here is the discription of the data set(which is also available in the notebook)
age: age of primary beneficiary

sex: insurance contractor gender, female, male

bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height,
objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9

children: Number of children covered by health insurance / Number of dependents

smoker: Smoking

region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.

charges: Individual medical costs billed by health insurance
### EDA
start with the standart . checking for `nan` and `duplicate` and how to handel them . after that get to know our data better and understand it's statistic information
after that get to the visualization
in `vis` part i investigate all colunms regard to the target (`charges`) and use other colunms as a color factor for other plots . 
continued with data engineering . creating new colunms and further drop colunms .
### preprocessing
in this part the `obj` colunms where encoded and standardization happen(it had a very low level of skewness which can be fixed by that) and of corse split into train and test sets and all ready for fitting a model
### model building
i chossed 3 models to work with . `randomforest` , `XGB` and `knneighbors` all as regressor . the hyperparameter of all three models were tuned and the best result was for XGB
### evaluation
i had another 3 metrics `r2_score` , `mean_absolute_error` , `mean_squared_error` in this three metrics XGB was again the best model so i pickel it .
there is more information in the notebook i suggest to read that.
