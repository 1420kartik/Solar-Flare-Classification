# Solar-Flare-Classification

## Introduction
Solar flares result from the sudden release of magnetic energy stored in the Sun, posing potential risks to Earth's communication and infrastructure. Extreme class imbalance and high-dimensional time series data pose challenges. The study aims to use MINIROCKET and other classifiers for real-time flare prediction.

## Data
The original data can be downloaded from https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/EBCFKM

The files created after statistical summarization (0_data_preprocessing.ipynb) - 
p1_data_new.csv
p2_data_new.csv
p3_data_new.csv
p4_data_new.csv
p5_data_new.csv

## Experiments
The following notebooks contain all the code and methodologies - 

#### 0_data_preprocessing.ipynb
This notebook carries out the dimension reduction technique using five statistical summarization calculations on the original SWAN-SF dataset.

#### 1_SVM_binary_and_all_class_classification.ipynb
#### 1_SVM_experiments_without_B_and_C_class_flares.ipynb
The notebooks mentioned above use the SVM classifier for all class classification and binary class classification on the dim-reduced data. We also perform the same experiment after removing B and C class flares instances.
Note - We only used dim-reduced data for SVM experiments.

#### 2_Minirocket_binary_and_all_class_classification.ipynb
#### 2_Minirocket_experiments_without_B_and_C_class_flares.ipynb
Using MINIROCKET classifier with same experiment settings.

#### 3_CIF_binary_and_all_class_classification.ipynb
#### 3_CIF_experiments_without_B_and_C_class_flares.ipynb
Using CIF classifier with same experiment settings.

#### 4_MRSEQL_all_experiments.ipynb
Using MRSEQL classifier with same experiment settings.

#### 5_LSTM_all_experiments.ipynb
Using LSTM classifier with same experiment settings.

#### 6_Visualization_boxplot.ipynb
#### 6_Visualization_lineplot.ipynb
Finally, we visualized all the results obtained by the above experiments using boxplots and lineplots.
