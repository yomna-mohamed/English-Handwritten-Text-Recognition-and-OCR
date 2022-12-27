# English-Handwritten-Text-Recognition-and-OCR
In this project a flexible convolutional neural network is proposed for text recognition. seeks to improve handwritten  text prediction using the Neural network on the OCR dataset  and the EasyOCR library to extract the whole text from the  handwritten text image, then compare it to our model to see if  we can outperform the existing EasyOCR model
Our simple model simulates the GRU decoder in EasyOCR
pre-trained model depending on two importantthings:
• Direction of English language ‘left to right’
• Region Of Interest ‘ROI’ by getting the effective
region of the image by calculating the change in
color between white and black and focusing on
black regions because it’s our target in the images.
After getting the important regions of the image we use our 
model to predict each character and combine them tocreate
an English word.
Tune hyperparameters of our model based on two
important things:
• Optimizer
• Learning Rate
And found that the best value for the learning rate was
0.01 and the best optimizer was ‘Adam’ so we build a
simple model with these hyperparameters.
We also add some regularization terms in our model
second model by adding:
• Batch Normalization Layer
• Layer Normalization Layer
