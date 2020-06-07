# MI-Segmentation Ver3.1

This is the official implementation code for [Deep learning for diagnosis of chronic myocardial infarction on nonenhanced cardiac cine MRI](https://pubs.rsna.org/doi/pdf/10.1148/radiol.2019182304).

Zhang, Nan*, Guang Yang*, Zhifan Gao, Chenchu Xu, Yanping Zhang, Rui Shi, Jennifer Keegan et al. "Deep learning for diagnosis of chronic myocardial infarction on nonenhanced cardiac cine MRI." Radiology 291, no. 3 (2019): 606-617.
* Co-first Author

If you use this code for your research, please cite our paper.

```
@article{zhang2019deep,
  title={Deep learning for diagnosis of chronic myocardial infarction on nonenhanced cardiac cine MRI},
  author={Zhang, Nan and Yang, Guang and Gao, Zhifan and Xu, Chenchu and Zhang, Yanping and Shi, Rui and Keegan, Jennifer and Xu, Lei and Zhang, Heye and Fan, Zhanming and others},
  journal={Radiology},
  volume={291},
  number={3},
  pages={606--617},
  year={2019},
  publisher={Radiological Society of North America}
}
```

## Requirements
This code is written for the Matlab (tested with versions R2014a-2014b) and Python (2.7) interpreter and requires the Matlab Image Processing Toolbox and the Keras.
- For the localization of the ROI, please download the [Faster-rcnn](https://github.com/jinfagang/keras_frcnn).
- Additionally, FullFlow is to download from https://cqf.io/fullflow/Full_Flow_Source_Code.zip
- Piotr's Matlab Toolbox (version 3.26 or later) written by Piotr Dollar is also required.

## Train New Dataset

To train a new dataset is also very simple and straight forward. Simply convert your cropped ROI by:
- 11x11_builder.m
- flow_builder.m

Then, running the train.py
