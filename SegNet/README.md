# model1

All batch normalizaton layer (BN layer) are from segNet Caffe
v1: segNet architecture initialized with 'msra' method (without class weights)
v2: segNet architecture initialized with preTrained weights (without class weights)
v3: segNet architecture initialized with preTrained weights and with class weights included.

preTrained weights are from segnet_pascal.caffemodel which can be downloaded in:
http://mi.eng.cam.ac.uk/~agk34/resources/SegNet/segnet_pascal.caffemodel

# model2

The v1, v2, and v3 are the same as these under model1. The only difference is the the batch normalization layer. 

Here, all the batch normalization layer(BatchNorm + Scale layers) are from official Caffe
