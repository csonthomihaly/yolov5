#!bin/bash
# Start in YOLOv5 folder:
python train.py --img 640 --batch 12 --epochs 1000 --data GTSDB.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs
