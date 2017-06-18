# Introduction

This project aims to release small convolutional neural networks as generic feature extractors for easy tasks 
(e.g. cat and dog classification) and fast inference in [Caffe](https://github.com/BVLC/caffe).

I think that using small models with similar accuracy as the [AlexNet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf) does can help us in fast training, 
fast fine tuning and fast inference in your applications which does not require big models such as [VGG](http://www.robots.ox.ac.uk/%7Evgg/research/deep_eval/), [Inception V3](https://github.com/soeaver/caffe-model) or [Resnet-50/101](https://github.com/BVLC/caffe/wiki/Model-Zoo#resnets-deep-residual-networks-from-msra-at-imagenet-and-coco-2015).

After doing some experiments, I found out [SqueezeNet](https://github.com/DeepScale/SqueezeNet) model is the fastest model with enough capacity for these purposes.

Also I considered [MobileNet](https://arxiv.org/abs/1704.04861). In Caffe, the naive implementation is using group parameter, however the speed is quite slow.
Right now I only use SqueezeNet.

The models are trained with ImageNet dataset and I got the following results in the validation set:

#TODO
