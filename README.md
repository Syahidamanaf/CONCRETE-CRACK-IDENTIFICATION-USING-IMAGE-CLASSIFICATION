# CONCRETE CRACK IDENTIFICATION USING IMAGE CLASSIFICATION
 
## DATASET

Description
The dataset contains concrete images having cracks. The data is collected from various METU Campus Buildings.
The dataset is divided into two as negative and positive crack images for image classification. 
Each class has 20000images with a total of 40000 images with 227 x 227 pixels with RGB channels. 
The dataset is generated from 458 high-resolution images (4032x3024 pixel) with the method proposed by Zhang et al (2016). 
High-resolution images have variance in terms of surface finish and illumination conditions. 
No data augmentation in terms of random rotation or flipping is applied. 

References:
2018 – Özgenel, Ç.F., Gönenç Sorguç, A. “Performance Comparison of Pretrained Convolutional Neural Networks on Crack Detection in Buildings”, ISARC 2018, Berlin.

Lei Zhang , Fan Yang , Yimin Daniel Zhang, and Y. J. Z., Zhang, L., Yang, F., Zhang, Y. D., & Zhu, Y. J. (2016). Road Crack Detection Using Deep Convolutional Neural Network. In 2016 IEEE International Conference on Image Processing (ICIP). http://doi.org/10.1109/ICIP.2016.7533052

## GOOGLE COLAB

The purpose of this project is to identify the concrete crack using Convolutional Neural Network(CNN). Google colab is used for this image classification problem with the application of Numpy, Pandas, and Tensorflow Keras.

## MODEL PREDICTION AND RESULT

This project is created by applying transfer learning method. VGG16 convolutional neural network is implemented here for the purpose of the project. VGG16 consists of 13 convolutional layers, 5 max-pooling layers and 3 fully connected layers. Classification layer then is added to create the entire model. Finally fine tuning is applied to improve the accuracy.

The model was trained with 5 epochs and produced training accuracy of 0.9966 and validation accuracy of 0.9962. In order to ensure the fine tune is working in improving the accuracy score, we trained the model with another 5 epochs and the result has a sligh improvement where the accuracy increase to 0.999 for training set and 0.988 for validation set.

Note: Fine tuning process is not required for this specific project because the accuracy using transfer learning itself is very good. Hence, it can be dismissed.

