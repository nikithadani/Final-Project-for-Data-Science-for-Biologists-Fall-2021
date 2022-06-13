# Final project for Data Science for Biologists, Fall 2021

This is a README file, written in _markdown_. README files are commonly part of disseminated software/code packages. They help to explain the contents of the software package: what files are what? how do you use the software? etc.

**[Instructions for final project](https://sjspielman.github.io/datascience_for_biologists/homeworks/project/project_proposal_instructions.html)**


I obtained the Breast Cancer cell data from the Kaggle website [here](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data), which also directs you to the UCI Machine Learning Repository [here](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29). The dataset contains 569 samples (357 benign and 212 malignant) of different features of breast tumor cell nuclei by using the biopsy method of fine needle aspirate (FNA) of a breasts mass. I picked this data set mainly because I actually wanted to learn what measurements are taken into consideration when doing biopsy on breast mass, I had no idea what exactly helps determine whether it is a malignant or benign breast tumor. Quite honestly by doing the model to predict future diagnosis, makes me feel successful in a way, even though my model is not being used for such important diagnosis, I feel like I can *actually* do models to keep pushing for better healthcare systems. 

The attributes in the data set are as follows:

+ id: Identifies the sample
+ diagnosis: Tumor is 1= Malignant or 0= Benign
+ radius: Mean of distances from center to points on the perimeter 
+ texture:  Standard deviation of gray-scale values 
+ perimeter: Distance around nuclear border  
+ area : Area of nucleus 
+ smoothness: Variation in the cell’s radial lengths  
+ compactness: perimeter$^2$ / area)
+ concavity: Size of indentations in the nuclear border
+ concave points: Number of concave portions of the nuclear border
+ symmetry: Deviation of nuclei shape from ideal 
+ fractal dimension: Measurement of nuclear border irregularity or "coastline approximation"
+ The mean(`variable_mean`), standard error(`variable_se`) and "worst" or largest (mean of the three
largest values, shown as `variable_se`) of these features were computed for each image,
resulting in 30 features. All feature values are recorded with four significant digits

Since the attributes have been explained above, the `variables` in the dataset are as follow:

+ `id`
+ `diagnosis`
+ `radius_mean`
+ `texture_mean`
+ `perimeter_mean` 
+ `area_mean`
+ `smoothness_mean`
+ `compactness_mean`
+ `concavity_mean`
+ `concave points_mean`         
+ `symmetry_mean `
+ `fractal_dimension_mean`
+ `radius_se`
+ `texture_se` 
+ `perimeter_se` 
+ `area_se`
+ `smoothness_se`
+ `compactness_se`
+ `concavity_se`
+ `concave points_se`
+ `symmetry_se`
+ `fractal_dimension_se`
+ `radius_worst` 
+ `texture_worst `
+ `perimeter_worst `
+ `area_worst`
+ `smoothness_worst` 
+ `compactness_worst` 
+ `concavity_worst `
+ `concave points_worst`
+ `symmetry_worst`
+ `fractal_dimension_worst`
+ `...33 `: This variable is full of NAs, it will be later deleted