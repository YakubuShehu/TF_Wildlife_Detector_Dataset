# TF Wildlife Detector Dataset

This is a dataset that I collected to train my own Wildlife detector with [TensorFlow's Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection).

It was generated for use with my MSc Thesis : *AN OPTIMIZED NEURAL-NETWORK BASED ALGORITHM FOR AUTOMATIC IDENTIFICATION AND QUANTIFICATION OF CONSERVANCY WILDLIFE ON HIGH RESOLUTION DRONE IMAGES*

> Due to time and resource limitations, we could not obtain a suitable amount of wildlife images from an aerial view. As a countermeasure, we decided to create/use simulations of wildlife from an "aerial-view", generated from 3D Models. These 3D-simulated images were then used as the image dataset for training and validation.
> In total, there are roughly 794 images of 3D-simulated wildlife.
> ```90% : 10% - Train : Test split``` 

## Getting Started

##### Folder Structure:
```
+ annotations: contains the xml files in PASCAL VOC format

+ data: contains the input file for the TF object detection API and the label files (csv)

+ images: contains the image data in .jpg/.png format

+ test_images_3D: contains the images used to test/validate the accuracy of single image inferences on 3D simulated wildife.

+ test_images_RW: contains the images used to test/validate the accuracy of single image inferences on 'Real World' wildlife.

+ training_checkpoints: contains custom exported training results and frozen inference graphs from various training results.

- a few handy scripts: generate_tfrecord.py is used to generate the input files
for the TF API and xml_to_csv.py is used to convert the xml files into one csv
```

## Copyright

See [LICENSE](LICENSE) for details.
Copyright (c) 2021 [Yakubu Shehu](https://wwww.yakubushehu.com/).

Inspiration from - Dat Tran's [Racoon Detector] (https://towardsdatascience.com/how-to-train-your-own-object-detector-with-tensorflows-object-detector-api-bec72ecfe1d9)