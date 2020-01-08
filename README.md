# Machine Learning Engineer Nanodegree
## Capstone Project 
## Image Detection for Facial Attribute - Smiling


#### Dataset: 
CelibA dataset is used for this project. 
http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html
However, for this project, it is downloaded (1.4GB) from the Kaggle website:
https://www.kaggle.com/jessicali9530/celeba-dataset
The size of the subset of this dataset used in this project is 99.6MB.


#### System used:
Windows 10 machine with 1.8GHz, 2401 Mhz, 2 Cores, 4 logical Processors
and  8 GB RAM


#### Software and Libraries used:
Python version 3.7.1 with Anaconda.
TensorFlow (CPU-only): https://www.tensorflow.org/install
##### Main Libraries:
- numpy
- pandas
- Keras
- tensorflow
- matplotlib



In order to replicate this project, the dataset needs to be downloaded from the Kaggle website: https://www.kaggle.com/jessicali9530/celeba-dataset
The folder structure is as follows:
```
capstone_project
      |---CelibA
      |        |---img_align_celeba
      |        |---list_attr_celeba.csv
      |        |---list_eval_partition.csv
      |---input
      |        |---dataset
      |        |         |---test
      |        |         |       |---0
      |        |         |       |---1
      |        |         |---train
      |        |         |        |---0
      |        |         |        |---1
      |        |         |---validate
      |        |         |        |---0
      |        |         |        |---1
      |        |---saved_models
      |        |         |---aug_models.weights.best.hdf5
      |        |         |---composite_model.hd5
      |        |         |---transfer_models_btnk_aug.weights.best.hdf5
      |        |         |---transfer_models_SGD.weights.best.hdf
      |        |         |---transfer_models.weights.best.hdf5
      |        |         |---weights.best.from_scratch.hdf5
      |---benchmark_model.ipynb
      |---benchmark_data_aug.ipynb
      |---capstone_report.pdf
      |---data_prep.ipynb
      |---transfer_learning_VGG19-SGD.ipynb
      |---VGG19-Transfer-BottleNeck-Aug.ipynb
      |---visualizations.ipynb
      |---proposal.pdf
```
Notes:
1. CelibA folder contains the dataset downloaded from Kaggle.
2. The cropped and aligned jpg images are available in the folder img_align_celeba
3. Input and subsequent folders (except for saved models) are created and the subset images are copied accordingly as described in data_prep.ipynb
4. The files under saved_models are created by running the appropriate notebooks.
5. benchmark_model.ipynb describes the benchmark model
6. benchmark_data_aug.ipynb describes the benchmark model with data augmentation as an improvement.
7. transfer_learning_VGG19-SGD.ipynb describes the model considering VGG19 compiled with SGD optimizer instead of rmsprop.
8. visualizations.ipynb has the visualizations for data augmentation and predictions.
9. VGG19-Transfer-BottleNeck-Aug.ipynb describes the final model (solution) which gives an accuracy of 90.64%

Due to the large file sizes, all the required files have not been uploaded. Please feel free to contact me for more details.
