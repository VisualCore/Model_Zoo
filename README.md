# SpectralMD_Model

  # FCN
  train.prototxt: architecture for training

  inference.prototxt: architecture for inference

  solver.prototxt: configuration file

  preTrained vgg-16 networks (refer to following link) are used to initialize this FCN architecture:

  caffemodel_url: http://www.robots.ox.ac.uk/~vgg/software/very_deep/caffe/VGG_ILSVRC_16_layers.caffemodel


  notes:
  'source: "/disk2/Faliu/fcn/data/train_combined.txt" ' within both train.prototxt and inference.prototxt refers to data in HDF5 format.     
  Please change this directory according to your data. The Caffe used is in: https://github.com/BVLC/caffe


  # SegNet
  # model1
  All batch normalization layers in segNet architecture under model1 folder are from segNet Caffe. That is, BN layer is used. 

  In this case, after finishing training segNet, the compute_bn_statistics.py should be conducted before testing segNet.

  Please refer to segNet tutorial website http://mi.eng.cam.ac.uk/projects/segnet/tutorial.html

  # model2
  All batch normalization layers in segNet architecture under model2 folder are from official Caffe.

  That is, BathNorm + Scale layers are used. In this case, there are only two steps which are segNet training and testing.

  notes: The segNet architectures under model1 are the same as that under model2. 

  The only difference is the bath normalization layer where one is from segNet Caffe (BN layer) and other one is from official Caffe (BathNorm + Scale layer). 

  The segNet Caffe used is in: https://github.com/alexgkendall/caffe-segnet

