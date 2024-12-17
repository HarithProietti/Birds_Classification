# Birds Classification

This project consisted in classifying pictures of birds, taken from different angles and with different resolutions.

My approach was the following : 

- Firstly, an object detection to just account for the part of the picture that actually contains the bird. Indeed, some pictures were taken from far away, for example birds on tree branches, hence the image would contain a lot of unnecessary parts. I used the Yolo model to perform this.
- Once the images were correctly cropped, I resized them to the same format, and trained a classifier to predict the classes. The model used was a Vision Transformer.

The training pipeline was done through Pytorch-Lightning. I also added data augmentation with pytorch.

This approach allowed me to get 86.5% on the test set, ranking top 24% of the competition.

