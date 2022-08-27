# Counting and classifying car using fine-tuned ViT in PyTorch

This is the final project of the deep learning course. During this project, first, a dataset of more than 500 Iranian car images from 3 different models ( Peugeot 206, Peugeot Pars, Pride)
is gathered by crawling images from car retail websites. Because the number of training examples is limited, we use a fine-tuned [Vision transformer](https://arxiv.org/abs/2010.11929) for classification. Besides, we use transfer learning with ResNet50 as another classification model. However, ViT model performs better than the ResNet50 model.
For counting purposes, we considered two different methodologies. Our first approach is to use the YOLO model to detect cars in an image and feed each detected car's image to the classification model. The final output would be the number of each car with its model.
The second counting method is based on regression and is proposed by [learning to count Everything](https://arxiv.org/abs/2104.08391), which used 147-FSC as a dataset. This model counts objects from any category, given only a few annotated instances from that category. 
