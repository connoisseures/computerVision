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
  - https://github.com/tensorflow/tensorflow/blob/master/tensorflow/tools/graph_transforms/README.md#introduction
  ```
  bazel build tensorflow/tools/graph_transforms:transform_graph
  ```
  - http://laid.delanover.com/how-to-freeze-a-graph-in-tensorflow/
+fine tune 
  - Choose a training regime that does not ruin the pre-trained weights, for example, **a lower learning rate** than for training from scratch.
  - https://www.tensorflow.org/hub/fine_tuning
+ https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/configuring_jobs.md  

Basic
---
+ https://towardsdatascience.com/epoch-vs-iterations-vs-batch-size-4dfb9c7ce9c9
+ http://cs231n.github.io/neural-networks-3/

Tutorial
---
+ https://www.tensorflow.org/alpha/tutorials/images/transfer_learning

+ Proto buffer
  - https://developers.google.com/protocol-buffers/docs/proto#simple

Q n A
---
+ manage restore session 
  - https://web.stanford.edu/class/cs20si/2017/lectures/notes_05.pdf
+ Training object detection model with multiple training sets 
  - https://github.com/tensorflow/models/issues/3031
```
train_input_reader: {
  tf_record_input_reader {
    input_path: ["PATH_TO_BE_CONFIGURED/train_a.record", 
                 "PATH_TO_BE_CONFIGURED/train_b.record"]
  }
  label_map_path: "PATH_TO_BE_CONFIGURED/label_map.pbtxt"
}
```

+ modify import files

```bash
        # for feature extractor 
        modified:   ../builders/model_builder.py
        # for frozen model 
        modified:   ../core/post_processing.py
        modified:   ../export_inference_graph.py
        modified:   ssd_squeezenet_feature_extractor.py
        modified:   ../../slim/nets/squeezenet.py

```
