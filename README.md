# Agriculture Crop Type Classification (Maize, Wheat, jute, rice and sugarcane) 


The main purpose of this project is to be able to find an architecture that can classify the above mentioned crops


Here are the list of thing that are available in the repository

- In **Project.ipynb** the original code is available, which we used for searching the suitable architecture
- In **Generate images.ipynb** the code is available that takes images and generates augmented images for your dataset (This can be helpful if dataset is small)

>It is assumed in given code that dataset and weights are already available in the required folders, the dataset needs to be present in the folder named as **dataset/crop_images** for training, **dataset/validation_crop_images** for validation, **dataset/test_crop_image** for testing.

The folders for the weights should be 

- **pre_trained_weights/model_1_weights.h5** for VGG 16, and it's available at https://drive.google.com/uc?id=1593tlRj2n5u19BNmIuQ5lz95jz8JGE9D
- **pre_trained_weights/model_2_weights.h5** for VGG 16, and it's available at https://drive.google.com/uc?id=159geg7BQoPR9WZfZQk1YTQ9OjVdTompt
- **pre_trained_weights/model_3_weights.h5** for VGG 16, and it's available at https://drive.google.com/uc?id=15CjkXjCuOm7x9RyuafDx9zy0lIjSc3y3

There are two types of weights in this dataset, first type of weights are the one that are trained based on the images generated by augmentation as the dataset contains very few images which are not enough for training, secondly the weights when the model was trained, so the test accuracy may be checked.

#Three types of models were used VGG16, ResNet, AlexNet 



# VGG 16
## The model for VGG 16 is given below
![NetworkDiagram.png](https://drive.google.com/uc?id=1rLopL_mXM-bRX7eRPkQr4ggp82BYZRXI)
  
The weights after training this model are available at https://drive.google.com/uc?id=15QQ-lOHzLHCjCS85aFFCi4KeXqyu1tC2
  
Given below are its results
| Number of epochs | Loss | Accuracy |
| ---------------- | ---- | -------- |
| 15               | 5.9  | 0.53     |
  
# ResNet
## The model for ResNet is given below
![NetworkDiagram.png](https://drive.google.com/uc?id=1dQbZ0TT7lmtJhQG1C55bBxuyo0F-fFmM)
  

The weights after training this model are available at https://drive.google.com/uc?id=15YoZnGL2txF7hTOQGACfR1rmjn2Knink
  
Given below are its results
| Number of epochs | Loss | Accuracy |
| ---------------- | ---- | -------- |
| 15               | 4.4  | 0.55     |
  
  
# Alex Net
## The model for Alex net is given below
  ![NetworkDiagram.png](https://drive.google.com/uc?id=136l8cPCXSnbDr_2M9AM-RJrDSoyqwEUM)
  
The weights after training this model are available at https://drive.google.com/uc?id=15zHvSgRl0NLUwR6k3bbugmVFCkWEDj3t
  
Given below are its results
| Number of epochs | Loss | Accuracy |
| ---------------- | ---- | -------- |
| 15               | 3.2  | 0.57     |
