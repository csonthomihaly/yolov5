#!bin/bash
# Start in YOLOv5 folder:
#python train.py --img 640 --batch 10 --epochs 10 --data DFG-tsd.yaml --weights yolov5s.pt --workers 6 --project Traffic_signs
#python train.py --img 640 --batch 10 --epochs 300 --data DFG-tsd.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs

# Cant use --cache ram <- not enough RAM in this PC
python train.py --img 640 --batch 10 --epochs 300 --data DFG-tsd.yaml --weights yolov5s.pt --workers 6 --project Traffic_signs

