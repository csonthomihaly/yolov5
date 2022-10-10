#!bin/bash
# Start in YOLOv5 folder:
python train.py --img 640 --batch 10 --epochs 1500 --data GTSDB.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs
