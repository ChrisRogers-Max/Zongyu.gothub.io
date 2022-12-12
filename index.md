## CNN Chest X-ray Disease Classifier (CCXrDC)
> ### Overview
CNN Chest X-ray Disease Classifier (CCXrDC) is a pure Python3-based software, aiming to classify users’ input chest X-ray images into four categories: Normal (healthy lungs), Tuberculosis (TB), COVID-19 infection and Bacterial/Viral Pneumonia (TB and COVID-19 infections are excluded) using convolutional neuron network (CNN) and VERY DEEP CONVOLUTIONAL NETWORK (VGG-11). The input image can be optionally segmented using U-Net based deep learning model, thereby sihfting the focus of subsequent classification model on the lung region. 

In order to enable the full function of our Graphical User Interface (GUI), downloading of the three models that we built up and trained are highly recommended, the links to their storage in Google Drive are provided:

* U-net based model for segmentation: [Best_model]
* Modified AlexNet for classification: [four_class_97_669_ac]
* VGG11 network for classification: [VGG11_model_second_colab]

[Best_model]: <https://drive.google.com/file/d/1PMb3sION8Pp42wVRi9KKmYCVi85pChMs/view?usp=sharing>
[four_class_97_669_ac]: <https://drive.google.com/file/d/10DC2YnbBLLGtl1VytyBtD4W8NZHRGZpQ/view?usp=sharing>
[VGG11_model_second_colab]: <https://drive.google.com/file/d/1RC-JFJfaTxqoNRhWDGwKFAVgge3Adjst/view?usp=sharing>

You are more than welcome to train our model in person. We've uploaded the code for the three networks construction in the names listed above. We've claimed the dataset we used for training segmentation and classifcation in our report. Do remember to adjust the filename of output model if you want to run the software with model you produce. 

If you don't feel like reading this documentation, here is the link of [the video tutorial] where one of our member concisely introduces how to use our software.

[the video tutorial]: <https://drive.google.com/file/d/17NkeixDznwnnUiTvEKkBAKd2TQUlL8aU/view?usp=share_link>

- - - -

> ### Environment Preparation
Virtual environments should be prepared in Python3 environment. We recommend to install the package manager [Anaconda] and then install an appropriate [PyTorch] and [TensorFlow] version that supports your device. 

[Anaconda]: <https://www.anaconda.com/>

[PyTorch]: <https://pytorch.org/>

[TensorFlow]: <https://www.tensorflow.org/>

>> #### Install packages 
Before using this software, you should make sure that your personal computer has all following necessary python packages installed. 
List of necessary packages and corresponding install script using pip install:
```
pip install numpy
```
```
pip install pillow
```
```
pip install scikit-image
```

```
pip install matplotlib
```

If you have further problems installing packages, we recommend you to visit this [website]

[website]: https://packaging.python.org/en/latest/tutorials/installing-packages/

- - - -

> ### Execution
This software has a  (GUI). There are two ways to launch the GUI. 
1. Run the programme by directly clicking the `python running` button 
2. In the python terminal: python GUI.py

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p1.png" width=80% height=80%>

>> #### Classify X-ray Images
In the GUI, click the `Input Image` and upload the chest X-ray image. CCXrDC supports input files of .jpg, .png and .jpeg. 
Choose the preferred model (VGG11 or CNN model) to classify pneumonia types.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p2.png" width=60% height=60%>

Click the `Determine` button, GUI will return a classification message and corresponding suggestions. If the result is COVID-19, a link to WHO guidance for self-management after COVID-19-related illness will appear on the right.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p3.png" width=60% height=60%>

>> #### Sharpen X-ray Images
Click the `Sharpen` button and a sharpened image will spontaneously appear. Click the `Save the image` button and you can save the processed image in your selected path.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p4.png" width=60% height=60%>

>> #### Segment X-ray Images
Click the `Segment` button and a segmented image will spontaneously appear. Click the `Save the image` button and you can save the processed image in your selected path.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p5.png" width=60% height=60%>

>> #### Video Tutorial (Help)
In the GUI, click the `HELP` button to watch a video tutorial.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p6.png" width=60% height=60%>

>> #### About us
Right-click the GUI to know us.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p7.png" width=60% height=60%>
<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p8.png" width=60% height=60%>

>> #### Quit
Click `QUIT` to close the program.

>> #### Warning/Conformation message
If no image is loaded or no model is chosen, a warning message will appear. 
A confirmation message will also appear before quitting the software by clicking the "x" button at the upper corner of the interface.

<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p9.png" width=60% height=60%>
<img src="https://github.com/ChrisRogers-Max/Zongyu.gothub.io/blob/master/Pictures/p10.png" width=60% height=60%>

- - - -

> ### Acknowledgements
CCXrDC thanks all used third-party libraries and previous works of Convolutional network construction.
