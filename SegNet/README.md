# model1

All batch normalizaton layer (BN layer) are from segNet Caffe

v1: segNet architecture initialized with 'msra' method (without class weights)

v2: segNet architecture initialized with preTrained weights (without class weights)

v3: segNet architecture initialized with preTrained weights and with class weights included.

preTrained weights are from segnet_pascal.caffemodel which can be downloaded in:

http://mi.eng.cam.ac.uk/~agk34/resources/SegNet/segnet_pascal.caffemodel

Three step: After finishing training segNet, the Scripts/compute_bn_statistics.py needs to be conducted, then go to segNet testing.

refer to: http://mi.eng.cam.ac.uk/projects/segnet/tutorial.html

# model2

The v1, v2, and v3 are the same as these under model1. The only difference is the the batch normalization layer. 

Here, all the batch normalization layer(BatchNorm + Scale layers) are from official Caffe

For batch normalization layer from official Caffe, the Scripts/compute_bn_statistics.py is unnecessary. 

After finishing segNet training, go to segNet testing directly.
