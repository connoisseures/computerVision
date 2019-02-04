
## reduce false positive

http://openaccess.thecvf.com/content_cvpr_2018/html/Cai_Cascade_R-CNN_Delving_CVPR_2018_paper.html

https://arxiv.org/pdf/1804.05197.pdf

http://openaccess.thecvf.com/content_cvpr_2018_workshops/w11/html/Yang_It_Takes_Two_CVPR_2018_paper.html

## DSSD

https://arxiv.org/abs/1701.06659

https://towardsdatascience.com/review-dssd-deconvolutional-single-shot-detector-object-detection-d4821a2bbeb5


## Tensorflow Object Detection API

https://github.com/tensorflow/models/tree/master/research/object_detection

### tutorial 

https://www.kdnuggets.com/2018/03/google-tensorflow-object-detection-api-the-easiest-way-implement-image-recognition.html

Here mAP (mean average precision) is the product of precision and recall on detecting bounding boxes. It’s a good combined measure for how sensitive the network is to objects of interest and how well it avoids false alarms. The higher the mAP score, the more accurate the network is but that comes at the cost of execution speed.

https://towardsdatascience.com/is-google-tensorflow-object-detection-api-the-easiest-way-to-implement-image-recognition-a8bd1f500ea0

https://medium.com/@sh.tsang

## notes 
By using SSD, we only need to take one single shot to detect multiple objects within the image, while regional proposal network (RPN) based approaches such as R-CNN series that need two shots, one for generating region proposals, one for detecting the object of each proposal. Thus, SSD is much faster compared with two-shot RPN-based approaches.


## Tensorflow ODAPI
### gen tfrecord 
https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/preparing_inputs.md

### notest
https://arxiv.org/pdf/1604.03540.pdf

the training set is distinguished by a large  imbalance  between  the  number  of  annotated  objects and the number of background examples (image regions not belonging to any object class of interest)

Unsurprisingly,  this is not a new challenge and a stan-dard solution, originally called bootstrapping
(and now of-ten called hard negative mining), has existed for at least 20 years.


