# Height-Weight-Regressor
Using Linear Regression to predict weight when height is given , as well as suggesting optimal weight using BMI
* Name - Ayush Agarwal 
* Details - IIT BHU Varanasi , ECE 
* Project - Height Weight Regressor 
* Skills - Linear Regressor , Supervised Learning , Machine Learning , Data Science 
* Tools - Google Colab Notebooks , Numpy , Pandas , MatplotLib , SeaBorn , SciKit-Learn 

## Dataset : 
The data was taken from Kaggle site : https://www.kaggle.com/datasets/mustafaali96/weight-height
I have also uploaded a copy of this dataset on this repository just in case this dataset is removed : https://github.com/ayush-agarwal-0502/Height-Weight-Regressor/blob/main/weight-height.csv .

## Data Preprocessing and Visualisation :

### Converting Lbs to Kg and inches to cm :

![image](https://user-images.githubusercontent.com/86561124/174354776-d671eb98-de84-42a0-98bb-34bd88f06432.png)

### Visualising the whole dataset :

![image](https://user-images.githubusercontent.com/86561124/174354903-b633031a-02b3-431b-a046-1c19037a13a8.png)

### Visualising separately for Male and Female :

![image](https://user-images.githubusercontent.com/86561124/174355047-002d94ed-5931-4a5c-85af-95381c4fa222.png)

The distribution of the data and the relation between height and weight clearly shows that __LINEAR REGRESSION__ would be optimal algorithm for the following problem .

### Checking Missing Values :

![image](https://user-images.githubusercontent.com/86561124/174355223-9ff30b53-2599-46dd-801e-a9562a5b7eed.png)

No missing values in the dataset . Hence no need to use Imputers .

### Checking Class Distribution in the Dataset :

![image](https://user-images.githubusercontent.com/86561124/174355373-0d30e701-60c3-4667-af64-5643ddcdd842.png)

Equal number of data samples for both male and female present , hence the dataset is well-balanced . No need to use Oversampling , Undersampling or SMOTE . 




