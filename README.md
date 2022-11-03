# Master-s-degree-end-of-study-project-

Breast cancer is the most frequent type of cancer in women and the second leading death cause worldwide. Early detection is an efficient way to diagnose and treat
breast cancer and also plays an important role in reducing mortality rates. In this
work, we proposed a breast cancer detection method that is based on segmentation information extracted by a segmentation model. Initially, we implemented a
segmentation model that has shown good results using the U-net and Res-Net. Secondly, we implemented several classification models. The first approaches are defined using pre-trained models, ResNet101, ResNet152, DenseNet169, MobileNet,
InceptionV3, and NasNet, and trained using 10-fold cross-validation, transfer Learning, and fine-tuning. DenseNet169 achieved the best results compared with the other
pre-trained models by 88.68% as average of validation accuracy, 71,11% as average
of test accuracy, and 79,9% as average of recall. While the second approach is defined by modifying the segmentation model in order to generate a label prediction
instead of generating a mask, it achieves an accuracy of 94%. Finally, we compared
the classification models based on the accuracy metric and visualization of predictions using Grad-CAM.

## Motivation
In this work, we focus on breast cancer as the second leading cause of death
for women worldwide. For evaluating the healthiness of the breast, radiologists
should find and notice the small details in order to detect an abnormality that may
be present in the organ. Sometimes, the detection can be difficult. That’s why it
is essential to have an automated method to help radiologists with breast cancer
assessment.

## Contributions
The goal of this work is to propose a breast cancer detection method by integrating the segmentation information extracted by a segmentation model in the classification model. The proposed method should improve the accuracy in breast mass
detection by completing the following Objectives :
• Training a segmentation model that will generate a predicted mask for every
case (mask with segmented mass for abnormal case or a black mask if it is a
normal case).
• Training a classification method for classifying images as normal or abnormal
using pre-trained models, ResNet101, ResNet152, DenseNet169, MobileNet,InceptionV3, and NasNet, with the use of Cross validation, transfer learning,
and Fine-Tuning in order to improve the accuracy.
• Creating a new model that is based on the pre-trained model of segmentation
that include the weights saved from the training of segmentation, and modification in the output part, and use it to classify mammograms in normal or
abnormal case.

![classification model](https://user-images.githubusercontent.com/66222519/199695058-1da03b9c-12b9-4b34-a461-444c90e1649e.png)
