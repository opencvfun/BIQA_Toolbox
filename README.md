# Introducetion
This Toolbox aims to provide relatively fair benchmark performances of several popular CNN architectures and some classical blind image quality assessment (BIQA) methods using hand-crafted features on four representative image quality assessment (IQA) datasets.


#### Main functions

1. `training_testing_CNNs.m` trains a CNN model using a proportion (e.g. 0.8) of images and test performance on the remaining images.

2. `crossDatasetTrainTest.m` trains a CNN model on one dataset and test performance on other datasets.

3. `evaluating_existing_methods.m` evaluates several representative classical BIQA methods including DIIVINE,CORNIA,BRISQUE, NIQE, IL-NIQE, HOSA and FRIQUEE. The source codes of some methods are too large to be included into this toolbox. You can first download and extract them into the ``supported_methods``.

**How to run the Code**

1. Download the MatConvNet into ``tools`` and Compile it according to the guidence on [website](http://www.vlfeat.org/matconvnet/)

2. Create a new fold ``pretrained_models`` and download the pre-trained [AlexNet](http://www.vlfeat.org/matconvnet/models/imagenet-caffe-alex.mat) or [ResNet](http://www.vlfeat.org/matconvnet/models/imagenet-resnet-50-dag.mat) into ``pretrained_models`` if necessary.

3. Create a new fold ``databases``. Download an IQA dataset into ``databases`` and extract the files. Currently, four datasets are supported including the LIVE Challenge, LIVE IQA, CSIQ and TID2013. 

4. Run any of the three main functions.



#### License

This toolbox is made available for research purpose only. 

We utilize the MatConvNet and libSVM toolboxes and re-implement some existing methods. Please check corresponding licence files for details.
