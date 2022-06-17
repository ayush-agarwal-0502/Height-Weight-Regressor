# Height-Weight-Regressor
Using Linear Regression to predict weight when height is given , as well as suggesting optimal weight using BMI
* Name - Ayush Agarwal 
* Details - IIT BHU Varanasi , ECE 
* Project - Height Weight Regressor 
* Skills - Linear Regressor , Supervised Learning , Machine Learning , Data Science 
* Tools - Google Colab Notebooks , Numpy , Pandas , MatplotLib , SeaBorn , SciKit-Learn 

## Code :
My code is availaible at : https://github.com/ayush-agarwal-0502/Height-Weight-Regressor/blob/main/height_weight_regressor_project.ipynb (in this repository itself) .

## Dataset : 
The data was taken from Kaggle site : https://www.kaggle.com/datasets/mustafaali96/weight-height

I have also uploaded a copy of this dataset on this repository just in case this dataset is removed : https://github.com/ayush-agarwal-0502/Height-Weight-Regressor/blob/main/weight-height.csv .

Please also look at the BMI and dataset analysis at bottom :)  .

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

## Prediction and Analysis :

![image](https://user-images.githubusercontent.com/86561124/174355824-d2780da2-f685-4530-9930-62bdebc66143.png)

### The Result :

![image](https://user-images.githubusercontent.com/86561124/174355912-3f90e509-b523-4ff7-a90a-a1fd0bc131b0.png)

The RMSE Score is in the range of 4 to 5 indicating that our model performed well here . 

### Successful TestRun :

![image](https://user-images.githubusercontent.com/86561124/174356209-8d1dcf72-3fe9-42c1-9682-8443726f82f7.png)

# But Wait , there is a catch :

The model is biased to the population samples we trained it on , this is not a fault but rather inherent of any Machine Learning System . So , how is my model exactly biased ??

### The BMI (Body Mass Index ) : 

For those of you who don't know , BMI (Body Mass Index ) is a measure of wellness of a person based only on height and weight of a person . 18.5 to 25 is called as the optimal (healthy) region .

![image](https://user-images.githubusercontent.com/86561124/174356997-6c257054-acef-46d7-92bd-45cf2c0edafe.png)

![image](https://user-images.githubusercontent.com/86561124/174357182-13a1650c-c83a-4a04-8c7e-2d077ec20675.png)

### Dataset Distribution :


![image](https://user-images.githubusercontent.com/86561124/174357579-8d035b8d-86eb-4e41-837e-dad1acda9e7d.png)

Here is the distribution for the heights and weights in the dataset :

![image](https://user-images.githubusercontent.com/86561124/174357622-a7b57569-7e94-4213-ba4f-b7fb66600499.png)
![image](https://user-images.githubusercontent.com/86561124/174357642-61ec4725-f5b4-4d1d-9514-bbd8d8b3b72c.png)

How does this affect the result u ask ? Well , here is the data plotted against BMI graph :

![image](https://user-images.githubusercontent.com/86561124/174358015-c892fd88-d1e8-4a38-a153-b430c122d2bc.png)

![image](https://user-images.githubusercontent.com/86561124/174357888-9ffe9faa-b218-48d0-9060-3fdc84cee265.png)
![image](https://user-images.githubusercontent.com/86561124/174357906-65d51f69-5ca8-4f59-b53b-cda2d5983726.png)

The zones between the lines in the graph indicate the different BMI zones respectively ( below lowest line would be less than 18.5 BMI , between first and second line from bottom is between 18.5 to 25 zone and so on ) . 

Since the actual data for females in the dataset is lying between 18.5 to 25 range , whereas for males the data is lying between 25 to 30 BMI range , hence the Regression Lines are also learnt close to those regions . 

__Hence the Machine Learning Model is bit biased to show the weights in males in Overweight Zone rather than normal zone , due to the Bias between male and female weigths in the given dataset/population__ . 









