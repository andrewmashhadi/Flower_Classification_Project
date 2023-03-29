# Flower Classification with Transfer Learning

In this code, I use the flower image dataset from Kaggle here: https://www.kaggle.com/datasets/alxmamaev/flowers-recognition. The data was collected from data flicr, google images, and yandex images. It contains 5 types of flowers: daisies, dandelions, roses, sunflowers, and tulips. Most of the images have resolution less than or equal to about 320x240 pixels.

I was able to train, tune/validate, and test a neural network model that leverages the structure and pretrained weights from the well-known ResNet50 model. I froze the ResNet weights and trained an additional hidden layer before making the final classification. This approach is generally referred to as "transfer learning".

The overall classification accuracy of this model was about 91%, with each class of flower reporting individual accuracies ranging from approximately 87% to 94%.

This code was used with Googles Compute Engine backend (GPU), containing roughly 40GB of vRAM. Google Drive was mounted to read/write files via drive.