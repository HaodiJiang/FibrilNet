# Tracing Hα Fibrils through Bayesian Deep Learning

Haodi Jiang, Ju Jing, Jiasheng Wang, Chang Liu, Qin Li, Yan Xu, Jason T. L. Wang and Haimin Wang

Institute for Space Weather Sciences, New Jersey Institute of Technology

## Abstract

We present a new deep-learning method, named FibrilNet, for tracing chromospheric fibrils in Hα images of 
solar observations. Our method consists of a data preprocessing component that prepares training data 
from a threshold- based tool, a deep-learning model implemented as a Bayesian convolutional neural network 
for probabilistic image segmentation with uncertainty quantification to predict fibrils, 
and a post-processing component containing a fibril- fitting algorithm to determine fibril orientations. 
The FibrilNet tool is applied to high-resolution Hα images from an active region (AR 12665) 
collected by the 1.6 m Goode Solar Telescope (GST) equipped with high-order adaptive optics 
at the Big Bear Solar Observatory (BBSO). We quantitatively assess the FibrilNet tool, 
comparing its image segmentation algorithm and fibril-fitting algorithm with those employed 
by the threshold-based tool. Our experimental results and major findings are summarized as follows. 
First, the image segmentation results (i.e., the detected fibrils) of the two tools are quite similar, 
demonstrating the good learning capability of FibrilNet. Second, FibrilNet finds more accurate 
and smoother fibril orientation angles than the threshold-based tool. Third, FibrilNet is faster than 
the threshold-based tool and the uncertainty maps produced by FibrilNet not only 
provide a quantitative way to measure the confidence on each detected fibril, 
but also help identify fibril structures that are not detected by the threshold-based tool 
but are inferred through machine learning. Finally, we apply FibrilNet to full-disk Hα images 
from other solar observatories and additional high-resolution Hα images collected by BBSO/ GST, 
demonstrating the tool’s usability in diverse data sets.

----
References:

Tracing Hα Fibrils through Bayesian Deep Learning. Haodi Jiang et al 2021 ApJS 256 20

https://iopscience.iop.org/article/10.3847/1538-4365/ac14b7

https://arxiv.org/abs/2107.07886


Requirements: 

Tensorflow-GPU 1.12.0, Keras 2.2.4, numpy 1.16.1, skimage 0.15.0, matplotlib 3.1.0, cv2 3.4.2, astropy 4.0.1. Please use the Jupyter Notebook to run the SolarUnet tool.

Usage: 

Run train.py to train the model. 
Run test.py to test the model.
