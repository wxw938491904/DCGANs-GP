# DCGANs-GP
Title: A 3D shale reconstruction technology based on DCGANs-GP

Authors: Ting Zhang, Xianwu Wang, Xin Ji, Yi DU


Email：wxw938491904@dingtalk.com

1.requirements


Tensorflow-gpu == 1.13.1
tensorlayer == 1.10.1


2.How to use？


First, preprocess the image: Cut the shale slice into 64*64*64 size pictures. Each training image consists of 64 pictures of size 64*64, stored in a separate folder. Then use use scripts/preparedata.py to convert the image into .npy format.


Secondly, set the network parameters such as batchsize, learning rate and storage location. The executable .py file of DCGANs-GP, the path is: DCGANS-GP/DCGANS-GPpy. After configuring the parameters and environment, you can run directly: python DCGANs-GP.py


Finally, in DCGANS-GP/savepoint/Test, find the loss images during the training process and the .npy format of the shale three-dimensional structure images of different rounds. Use scripts/loadnpy to convert .npy to .txt format for later analysis and processing.
