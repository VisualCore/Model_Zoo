# Model_Zoo

# FCN
  train.prototxt: architecture for training
  
  inference.prototxt: architecture for inference
  
  solver.prototxt: configuration file
  
  vgg16-fcn.caffemodel: pre-trained model
  
  _iter_10000.caffemodel: final trained model with previous architecture

notes:
source: "/disk2/Faliu/fcn/data/train_combined.txt" in both train.prototxt and inference.prototxt is the used data in HDF5 format. Please change this directory according to your data.


# SegNet
