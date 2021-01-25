# Loan Classification

The purpose of this project is to build an ANN model, trained to predict whether new potential customers will pay back their loan.

## Dataset
Download [this data](https://www.kaggle.com/wordsforthewise/lending-club) from Kaggle.
There are 151 columns in this data. 
[preprocessing script](https://github.com/taishi-nammoto/loan-classification/blob/main/preprocessing.ipynb) allows you to trim the majority of irrenevant features. 

## Installation
```
pip install tensorflow==2.4.0
pip install matplotlib==3.1.1
pip install pandas==0.25.2
pip install scikit-learn==0.21.3
pip install seaborn==0.9.0
```

## Model Summary
[main script](https://github.com/taishi-nammoto/loan-classification/blob/main/preprocessing.ipynb) allows you to tarin and test the model below with the preprocessed dataset. 

```
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense (Dense)                (None, 807186, 65)        4290      
_________________________________________________________________
dropout (Dropout)            (None, 807186, 65)        0         
_________________________________________________________________
dense_1 (Dense)              (None, 807186, 30)        1980      
_________________________________________________________________
dropout_1 (Dropout)          (None, 807186, 30)        0         
_________________________________________________________________
dense_2 (Dense)              (None, 807186, 15)        465       
_________________________________________________________________
dropout_2 (Dropout)          (None, 807186, 15)        0         
_________________________________________________________________
dense_3 (Dense)              (None, 807186, 1)         16        
=================================================================
Total params: 6,751
Trainable params: 6,751
Non-trainable params: 0
_________________________________________________________________
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
