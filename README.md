# Deep Dream

As inspired and instructed by https://github.com/google/deepdream

# Directions

## Installation

Clone this repo into a directory on your machine, and also clone the [Caffe repo](https://github.com/BVLC/caffe) in a directory parallel to this one. 

Make sure you have at least one caffe model downloaded and placed in the corrct model path in this caffe repo. For example, I used the GoogleNet model, identified as [bvlc_googlenet.caffemodel](http://dl.caffe.berkeleyvision.org/bvlc_googlenet.caffemodel), and placed in /caffe/models/bvlc_googlenet.

Ensure you have Python installed on your machine and accessible via your system path. 

Install the dependencies as specified in the [Deep Dream Notebook](https://github.com/google/deepdream/blob/master/dream.ipynb). Using MacPorts, I installed these dependencies using this command:

`sudo port install caffe py-numpy py-ipython py-pil py-scipy py-protobuf`

## Running the script

From the command line, type:

`python app.py [filename]`

where `[filename]` is the full name of an image file located in the same directory as the script. If you don't supply a `[filename]` argument, the script will use a default file, as specified in the script