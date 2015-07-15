# Deep Dream

As inspired by https://github.com/google/deepdream

# Directions

## Installation

Clone this repo into a directory on your machine, and also clone the [Caffe repo](https://github.com/BVLC/caffe) in a directory parallel to this one.

Ensure you have Python installed on your machine and accessible via your system path. 

Ensure you have the dependencies installed as specified in the [Deep Dream Notebook](https://github.com/google/deepdream/blob/master/dream.ipynb). Using MacPorts, I installed these dependencies using this command:

`sudo port install caffe py-numpy py-ipython py-pil py-scipy py-protobuf`

## Running the script

From the command line, type:

`python app.py [filename]`

where [filename] is the full name of an image file located in the same directory as the script. If you don't supply a [filename] argument, the script will use a default file, as specified in the script