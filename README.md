# dp-posthoc repository contents
This repository is a preliminary but novel examination into how differential privacy affects existing methods of post hoc model explanation. It includes a juptyer notebook which examines the impact of differential privacy on the LIME explanation method when used for a residual neural network. For more of an in depth motivation behind this repo as well as background on differential privacy and LIME are, please refer to the dp-posthoc-paper pdf. For areas of future work, please also refer to the dp-posthoc-paper.pdf. 
# notebook contents 
The CIFAR10 (https://www.cs.toronto.edu/~kriz/cifar.html) dataset is used to train RESNET18 models (https://pytorch.org/vision/main/models/generated/torchvision.models.resnet18.html) with and without differential privacy. The OPACUS privacy engine (https://opacus.ai/tutorials/building_image_classifier) is used to implement differential privacy. The LIME method of explanation (https://captum.ai/tutorials/Image_and_Text_Classification_LIME) is then used to generate predictions in the form of heatmaps that display which features of the images are most important in classifying the image. The goal is to observe differences in explanations for models with and without differential privacy. The notebook also includes an untrained model as a baseline to more accurately guage image variation relevance. 

