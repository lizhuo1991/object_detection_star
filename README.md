# object_detection_reproduction
the reproduction of object detection

Faster RCNN: 
- https://github.com/endernewton/tf-faster-rcnn (the best)

- https://github.com/rbgirshick/py-faster-rcnn
- https://github.com/akshaylamba/FasterRCNN_KERAS
- https://github.com/eric612/Vehicle-Detection
- https://github.com/CharlesShang/FastMaskRCNN

# VGG.npy
- 链接：https://pan.baidu.com/s/1tbeZgYEbuQYdSAcdmrX-fg 密码：bh96
- https://pan.baidu.com/s/1zctm_3yezrPPft7kOxW2_g

# 基础tensorflow模型下载：
- https://github.com/tensorflow/models/tree/master/research/slim

# Read tensor name and weight values from .ckpt file:
- https://blog.csdn.net/qq_32331347/article/details/79048899

# Reproduction of tf-faster-rcnn:
- Create a soft link to use the VOC datasets in data folder

ln -s [VOC datasets folder] [current code data folder]

- Report errors from line 122 and 129 of voc_eval.py

line 122 error is python version problem, change line 121 to -- with open(cachefile, 'wb') as f: --

line 129 error, change line 105 to -- cachefile = os.path.join(cachedir, '%s_annots.pkl' % imagesetfile.split("/")[-1].split(".")[0]) --
