---
layout: post
publish: true


---
### Caffe overview
- Writen in c++

- document sometimes out of Date

- Don't be afraid to read the code

- **convnet**

### Four Major classes

- Blob: Stores data and derivatives

- data and diffs

- Layer: Tranfroms bottom blobs to top blobs

- Look at code

- Net: many layers: computes gradients via forward/backward

- Solver: Uses gradients to update weights

### Cafe Protocol Buffers

.proto file

- Typed json

Serializa instances to text file

Compile classes for different languages
(widely used in caffe)

caffe.proto

### Training/Finetuning

1. Convert data(run a script)

2. Define net(edit prototxt)

3. Define solver(edit prototxt)

4. Train()

### Convert data
LMDB

Windows

From memory

### Define Net
layers

Not compositional : can't easily define a residual

### finetuning
Keep value pairs

match the name

reinitialize

### Define solver

### Train

-gpu all for multi-GPU Training

### Complex initialization: can't/hard

Caffe: Model Zoo

AlexNet, VGG, GoogleNet, ResNet,

### Python interface

read the code : caffe/python/caffe/_caffe.cpp_

caffe/python/caffe/pycaffe.py

Good for:
interface with numpy

Extract features: Run net forward

Compute gradients： run net backward

Define layers in Python with numpy(CPU only)

### Caffe Pros/const

+ Good for feedforward networks

+ Good for finetuning existing networks

+ Need to write C++/CUDA for new GPU layers

Cross-validation

### Torch

personal

### overview
facebook, NUY

### Torch:Lua

High level scripting languages, easy to interface with code

Similar to Javascript

1-index

Torch: Tensors

Torch tensors are just like numpy array

almost one-to-one from numpy to tensor

###

like numpy can't easily change data type

Unlike numpy,GPU is just a datatype away

Documentation on GitHub: not super complete but Good

### nn

nn models lets you easily build and train neural net

### Torch:cunn

Runing on GPU is easy

adam and RMS

### Torch:optim

Write a callback function that return loss and gradients

### Torch: moduls

Caffe has Nets and layers

Torch just has modules

forward: updateOutput

Tons of modules and loss functions

Write your own modules is easy

###

Container modules allow you to combine multiple modules

Sequential/ConcatTable

Use nngraph to build modules that combine their unputs in complex ways

symbolic variable

### Torch: Pretrained models

loadcaffe

use luarocks

### Typical Workflow

1. Preprocess data
2. Train

### Pro/cons
- Lua

- Less plug-and-play

- Not great for RNN

### Theano

From Yoshua Bengio group at University of Montreal

High-level Keras,L
