#!bin/bash
# Start in YOLOv5 folder:
#python train.py --img 640 --batch 10 --epochs 10 --data DFG-tsd.yaml --weights yolov5s.pt --workers 6 --project Traffic_signs
#python train.py --img 640 --batch 10 --epochs 300 --data DFG-tsd.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs


#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights yolov5s.pt --workers 20 --cache ram --device 0,1 --project Traffic_signs

# Resume trained weight

#python train.py --img 640 --batch-size 64 --epochs 2000 --data DFG-tsd.yaml --weights Traffic_signs/exp10/weights/best.pt --workers 20 --cache ram --device 0,1 --project Traffic_signs

# Start from original v5s weight with correct splitting & batch 64
python train.py --img 640 --batch-size 64 --epochs 2000 --data DFG-tsd.yaml --weights yolov5s.pt --workers 10 --cache ram --device 0,1 --project Traffic_signs
