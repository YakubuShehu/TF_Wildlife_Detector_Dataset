# TF Wildlife Detector Dataset

This is a dataset that I collected to train my own Wildlife detector with [TensorFlow's Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection).

> Due to time and resource limitations, the image dataset of wildlife used for training and validation, are from simulations generated from 3D Models. In total, there are roughly 794 images.
```90% : 10% - Train : Test split``` 

## Getting Started

##### Folder Structure:
```
+ annotations: contains the xml files in PASCAL VOC format

+ data: contains the input file for the TF object detection API and the label files (csv)

+ images: contains the image data in .jpg/.png format

+ training_checkpoints: contains custom exported training results and frozen inference graphs from various training results.

- a few handy scripts: generate_tfrecord.py is used to generate the input files
for the TF API and xml_to_csv.py is used to convert the xml files into one csv
```

## Copyright

See [LICENSE](LICENSE) for details.
Copyright (c) 2021 [Yakubu Shehu](https://wwww.yakubushehu.com/).

Inspiration from - Dat Tran's [Racoon Detector] (https://towardsdatascience.com/how-to-train-your-own-object-detector-with-tensorflows-object-detector-api-bec72ecfe1d9)