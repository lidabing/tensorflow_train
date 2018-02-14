# tensorflow_train

```
python object_detection/dataset_tools/create_pet_tf_record.py 
--label_map_path=object_detection/data/pet_label_map.pbtxt
--data_dir=D:/works/tensorflow/models/research --output_dir=D:/works/tensorflow/models/research
```

```
python object_detection/train.py \
--logtostderr \
--pipeline_config_path=D:/works/tensorflow/TensorFlow_Custom_ObjectDetection_/models/model/ssd_mobilenet_v1_coco.config \
--train_dir=D:/works/tensorflow/TensorFlow_Custom_ObjectDetection_/train
```

```
python object_detection/export_inference_graph.py  --input_type image_tensor   --pipeline_config_path D:/works/tensorflow/TensorFlow_Custom_ObjectDetection_/models/model/ssd_mobilenet_v1_coco.config --trained_checkpoint_prefix D:/works/tensorflow/TensorFlow_Custom_ObjectDetection_/train/model.ckpt-21925 --output_directory D:/works/tensorflow/TensorFlow_Custom_ObjectDetection_/out
```


```
tensorboard --logdir=D:\works\tensorflow\TensorFlow_Custom_ObjectDetection_\train
```
