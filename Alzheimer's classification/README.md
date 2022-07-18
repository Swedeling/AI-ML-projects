# Classification of changes related to Alzheimer's disease on MRI

The aim of the study was to find a classification algorithm with the highest possible accuracy that could be used as a tool for Alzheimer's disease severity diagnosis based on MRI brain images.

## Introduction 



## Database

The goal of this project was to best match brain images to the appropriate Alzheimer class. The dataset I used can be found at the URL: [Kaggle](https://www.kaggle.com/datasets/sachinkumar413/alzheimer-mri-dataset). The dataset contains 6400 MRI images of brain with varying degrees of alzheimer's disease. There are also images of healthy brain in the dataset which will also serve us in the learning process.

## Methods

I decided to create 5 different CNN models and study the effect of parameters on the results. In addition, I also tried another approach by checking how logistic regression would perform. All models can be viewed in detail in [the notebook]('Alzheimer's classification\Alzheimer's classification.ipynb'). 

## Results
Detailed results can be found in the notebook (precision, recall, F1-score, confusion matrix). Below only a short summary of accuracy for each method: 

| Model  | Accuracy |
| ------------- | ------------- |
| CNN I  | 0.99 |
| CNN II  | 0.99  |
| CNN III  | 0.99  |
| CNN IV  | 0.93  |
| CNN V  | 0.85  |
| LR I  | 0.45 |
| LR II  | 0.45  |

## Conclusions and future explorations 
At the end I can say that:
* Convolutional network is good solution for Alzheimer's disease severity classification based on the MRI images
* the best results are for the first three models 
* I recommed first model, because it is the simplest one
* VGG16 architecture is not the best option in this case
* A complex model is not necessary to solve the design problem 
* Logistic Regression is not good option in this case
* satisfactory results have been achieved (99%)


## Bibliography

[1] [Kaggle Dataset](https://www.kaggle.com/datasets/sachinkumar413/alzheimer-mri-dataset)