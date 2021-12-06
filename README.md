# MIST

[Project](https://github.com/jiayipan/MIST-net) | [Arxiv](https://arxiv.org/abs/2111.14831) .

### Citation
If you use this code for your research, please cite our paper:

```
bib.....
```

Issue: The sparse-view data reconstruction is one of typical underdetermined inverse problems, how to reconstruct high-quality CT images from dozens of projections is still a challenge in practice. 

Goal: To address this challenge, in this article we proposed a Multi-domain Integrative Swin Transformer network (MIST-net).

Features: 

(1) The MIST-net incorporated lavish domain features from data, residual-data, image, and residual-image using flexible network architectures. Here, the residual-data and residual-image domains network components can be considered as the data consistency module to eliminate interpolation errors in both residual data and image domains, and then further retain image details. 

(2): To detect the image features and further protect image edge, the trainable Sobel Filter was incorporated into the network to improve the encode-decode ability. 

(3). With the classical Swin Transformer, we further designed the high-quality reconstruction transformer (i.e., Recformer) to improve the reconstruction performance. The Recformer inherited the power of Swin transformer to capture the global and local features of the reconstructed image. 



### Install dependencies
cuda=11.1, python=3.8, torch=1.8
Before trainng, you should install a library named CTLIB. Run

```
python setup.py install
```

###  Own datasets
To train mist-net model on your own image, we may need generate datasets. Run

```
python fbpanglepro2imgtest.py
```


###  Train and Test
Run

```
python mainMISTnet.py
```


### Results
see [paper](https://arxiv.org/ftp/arxiv/papers/2111/2111.14831.pdf) .
