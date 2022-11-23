#!bin/bash
# Start in YOLOv5 folder:
#python train.py --img 640 --batch 10 --epochs 1500 --data GTSDB.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs

#python train.py --img 640 --batch-size -1 --epochs 2000 --data GTSDB.yaml --weights '' --cfg 'yolov5x_43.yaml' --workers 22 --cache ram --device 0,1 --project Traffic_signs_v5x_scratch_GTSDB

python train.py --img 640 --batch -1 --epochs 2000 --data GTSDB.yaml --weights yolov5x.pt --cache ram --workers 22 --device 1 --project Traffic_signs_v5x_GTSDB
