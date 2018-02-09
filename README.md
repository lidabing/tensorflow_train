# tensorflow_train

```
python object_detection/dataset_tools/create_pet_tf_record.py 
--label_map_path=object_detection/data/pet_label_map.pbtxt
--data_dir=D:/works/tensorflow/models/research --output_dir=D:/works/tensorflow/models/research
```

```
python object_detection/train.py \
--logtostderr \
--pipeline_config_path= D:/training-sets /data-translate/training/ssd_mobilenet_v1_pets.config \
--train_dir=D:/training-sets/data-translate/training
```

```
python object_detection/export_inference_graph.py 
--input_type image_tensor 
--pipeline_config_path D:\works\tensorflow\models\research\data\faster_rcnn_resnet101_pets.config 
--trained_checkpoint_prefix D:\works\tensorflow\models\research\train/model.ckpt-12421 
--output_directory D:\works\tensorflow\models\research\out
```
