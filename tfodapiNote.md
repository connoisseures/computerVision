Notes on TensorFlow Object Detection API
===

https://github.com/tensorflow/models/tree/master/research/object_detection

Framework
---
+ Main Flow 
  - Running the Training Job
  - Running Tensorboard
  - https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/running_locally.md
+ create a new model
  - https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/defining_your_own_model.md
+ Freezing Model
  - https://cv-tricks.com/how-to/freeze-tensorflow-models/
  - https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/exporting_models.md
  - 
+fine tune 
  - Choose a training regime that does not ruin the pre-trained weights, for example, **a lower learning rate** than for training from scratch.
  - https://www.tensorflow.org/hub/fine_tuning
  
Q n A
---
+ manage restore session 
  - https://web.stanford.edu/class/cs20si/2017/lectures/notes_05.pdf
