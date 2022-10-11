# License-plate-detection
build license plate detection using Transfer Learning technique + applying easyocr to get the license numer. it can be used in automatic parking management
i have used the license plate dataset from kaggle https://www.kaggle.com/code/sayamkumar/car-license-plate-detection.

I have tried 2 architecture mobillnet and retinanet50 and i have used two style of transfer learning
(fine tune the whole model, or use eager few shot to train the classification and detection box)


After the training and evaluation of our model. I Test it on algerian license plate  and it work very good.
with adding some regular text expression tho match the algerian license numbering, like the first part contain 5 or 6 numbers and so on.

finally i freezed the model and export it into tfjs and tflite versions.
