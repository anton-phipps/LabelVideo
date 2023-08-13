The steps to train and export the labels goes as follows:

01. First change your .tif files to .png files so they can be properly labeled

02. Use YBAT to create the labels. Export to coco for .json format needed in the training step

03. Train the model with the trainRCNN notebook. Place the images in the images folder and the labels in the label folder just for organization sake. The model is designed to be saved in the model folder. Then that can be copied to the model folder of the label-creator

04. Place your files which you want labeled in the videoFiles folder, and the model from the last step in the model folder. There is a max value for the box y dimension and x dimension which can be adjusted to remove some false positives from the final label.


File used for original labels: 'agar sw 1 (unmasked).tif'