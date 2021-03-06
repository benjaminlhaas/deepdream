# Deep Dream

As inspired and instructed by https://github.com/google/deepdream

# Directions

## Installation

Clone this repo into a directory on your machine, and clone the [Caffe repo](https://github.com/BVLC/caffe) into a directory parallel to that.

Make sure you have at least one caffe model downloaded and placed in the corrct model path in the caffe repo from the previous step. For example, I used the GoogleNet model, identified as [bvlc_googlenet.caffemodel](http://dl.caffe.berkeleyvision.org/bvlc_googlenet.caffemodel), and placed it in /caffe/models/bvlc_googlenet.

Ensure you have Python installed on your machine and accessible via your system path. 

Install the dependencies as specified in the [Deep Dream Notebook](https://github.com/google/deepdream/blob/master/dream.ipynb). Using MacPorts, I installed these dependencies using this command:

`sudo port install caffe py-numpy py-ipython py-pil py-scipy py-protobuf`

## Generating images

From the command line, type:

`python app.py [filename]`

where `[filename]` is the full name of an image file located in the same directory as the script. If you don't supply a `[filename]` argument, the script will use a default file, as specified in the script.

The script will save output image files to disk, either in the root level, or in the 'frames' directory.

## Notes

The file `caffe_layers.txt` file is the listing of all available caffe layers (it is the output of running `net.blobs.keys()`)
