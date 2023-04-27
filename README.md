# Automatic-License-Plate-Detection-and-Extraction

At the start of the project, we require software IDE to begin working on the project. Some recommended IDEs are Anaconda and the zip file containing LabelIMG. Please note that the dataset for the project is not provided, but you can create your own dataset. Once Anaconda is downloaded, you will need to execute specific commands.



Commands:  "conda install -c anaconda lxml" Before you are typing the command in conda prompt you need to be in labelIMG directory(i.e where the project is saved locallly)
"pyrcc5 -o libs/resources.py resources.qrc" Same as the before command you need to verify the directory (i.e It should be in LabaelIMG)


After succesfull run you need to run the command: "python labelImg.py" It opens the labeling editors and you need to label the images.

Once the image labeling process is completed, the next step is to begin data preprocessing. This involves verifying the .xml files that were extracted during the image labeling process.

During data preprocessing, you will verify whether the images have been processed correctly or not. Once you have ensured the correctness of the processed images, the next step is to convert the .xml files to .csv files. In these .csv files, you can access the coordinates of the objects that you have labeled.

Once the conversion of .csv file is completed, the next step is to begin training the data to detect the object. Please note that the epoch value can be set according to your dataset (i.e images), and it is important to confirm the time interval as well. After training the model, the next step is to continue building the deep learning model.

In the deep learning model, we pass the pipeline of code to predict the object in the correct position. After sending a sample image through the pipeline, if the number plate is detected correctly, it means that the code is running successfully. However, if the number plate is not detected correctly, you may need to train the model more and more. It is also important to check the path and directories in the code to ensure that they are correct.

After completing object detection, the next step is to integrate the OCR algorithm into the deep learning model to extract characters from the number plate. However, please note that in our code, the OCR algorithm only recognizes English characters. It is worth noting that OCR algorithms can recognize more than 26 languages. Also, it is important to keep in mind that the OCR algorithm only works when the image is at a certain angle and with a certain level of clarity. If the image does not meet these requirements, the OCR algorithm may not work accurately.
