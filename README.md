# DCGANs-GP
A 3D shale reconstruction technology based on DCGANs-GP

1.requirements
Tensorflow-gpu == 1.13.1
tensorlayer == 1.10.1

2. How to use？
First, preprocess the image: cut the image into 64*64*64 size, and use scripts/preparedata.py to convert the image into .npy format.
Secondly, set the network parameters such as batchsize, learning rate and storage location. The executable .py file of DCGANs-GP, the path is: DCGANS-GP/DCGANS-GPpy. After configuring the parameters and environment, you can run directly: python DCGANs-GP.py
Finally, in DCGANS-GP/savepoint/Test, find the loss images during the training process and the .npy format of the shale three-dimensional structure images of different rounds. Use scripts/loadnpy to convert .npy to .txt format for later analysis and processing.
