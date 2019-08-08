Projects 
===

### scene understanding 

+ we address the problem of localizing and recognition of functional areas from an arbitrary indoor scene, formulated as a two-stage deep learning based detection pipeline evaluation.

    - in the project, we replace the two-stage pipeline by Faster-RCNN, which gives region proposal and then classifies the region.
    - use VGG as the backbone of Faster-RCNN.

+ main contributions of this paper are as follows: 
    1. a scene functional area ontology for indoor domain;
    2. the first two stage, deep network based recognition approach is developed and presented for scene functional understanding,
        - I use Faster-RCNN to replace two state pipeline
    3. the first scene functionality dataset is compiled and made publicly available, which contains more than 100,000 annotated training samples and two sets of testing images from different indoor scene

+ approach 
    1. a deep neural network is trained to take each of these areas as input and output a belief distribution over the ontology of scene functional areas
    2. the final output of our system is visualized. Bounding boxes are used to indicate the detected location of the functional area and different color is used to indicate the function predicted.


