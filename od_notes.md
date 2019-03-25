Object Detector
---

SSD
---
+ SSDs do not need an initial object proposals generation step. This makes it, usually, faster and more efficient than two-stage approaches such as Faster R-CNN, although it sacrifices performance for detection of small objects to gain speed.
+ Also, deconvolutional layers are used in the detection part to increase the resolution of the feature maps produced by the feature extractor. This would theoretically allow for better detection of small objects by providing additional large-scale context.
+ https://medium.com/@amadeusw6/variations-of-ssd-understanding-deconvolutional-single-shot-detectors-c0afb8686d03

## notes 
By using SSD, we only need to take one single shot to detect multiple objects within the image, while regional proposal network (RPN) based approaches such as R-CNN series that need two shots, one for generating region proposals, one for detecting the object of each proposal. Thus, SSD is much faster compared with two-shot RPN-based approaches.
