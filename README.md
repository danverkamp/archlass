archlass
==============================

Architectural classification of homes based on images.

A Convolutional Neural Network for binary classification was trained using Victorian and Craftsman style houses as inputs.  Images were downloaded from the internet, with some basic preprocessing to remove images that were not of homes (manually at first, with some attempts made at automatic bad image removal using a pretrained CNN).  Finally, sizes were standardized.  Training data was augmented using shear, horizontal flip, and zoom.  

Preprocessing is done in the ```Preprocess.ipynb``` notebook.  All model training is done in the ```Train Model.ipynb``` notebook in the notebook directory.  Finally, ```Visualize Model.ipynb``` explores some of the model structure, as well as performance on out of sample images (mainly grabbed from Google Maps).  

A few are seen below: 

![OOS Predictions](/reports/figures/out_of_sample_predictions.png)

An attempt was made to visualize filter sensitivity using ([Keras: Convolution Filter Visualization](https://keras.io/examples/conv_filter_visualization/)): 

![Filter Sensitivity](reports/figures/model_conv2d_2_3x3.png)

And activations were visualized to a Crafstman home: 

![Conv 1](rhttps://github.com/danverkamp/archlass/blob/master/reports/figures/conv_layer_1.png)

Project organization based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
