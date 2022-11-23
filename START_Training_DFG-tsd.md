#!bin/bash
# Start in YOLOv5 folder:
#python train.py --img 640 --batch 10 --epochs 10 --data DFG-tsd.yaml --weights yolov5s.pt --workers 6 --project Traffic_signs
#python train.py --img 640 --batch 10 --epochs 300 --data DFG-tsd.yaml --weights yolov5s.pt --cache ram --workers 6 --project Traffic_signs


#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights yolov5s.pt --workers 20 --cache ram --device 0,1 --project Traffic_signs

# Resume trained weight

#python train.py --img 640 --batch-size 64 --epochs 2000 --data DFG-tsd.yaml --weights Traffic_signs/exp10/weights/best.pt --workers 20 --cache ram --device 0,1 --project Traffic_signs

## Correct trainings

# Start from original v5m weight with correct splitting & batch 64
#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights yolov5m.pt --workers 16 --cache ram --device 0,1 --project Traffic_signs_v5m

# Start from original v5s weight with correct splitting & batch 64
#python train.py --img 640 --batch-size 64 --epochs 2000 --data DFG-tsd.yaml --weights yolov5s.pt --workers 10 --cache ram --device 0,1 --project Traffic_signs

# Start from original v5n weight with correct splitting & batch 64
#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights yolov5n.pt --workers 16 --cache ram --device 0,1 --project Traffic_signs_v5n

# Start from scratch v5m weight with correct splitting & batch 64
# python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights '' --cfg 'yolov5m_200.yaml' --workers 16 --cache ram --device 0,1 --project Traffic_signs_v5m_scratch

# Start from scratch v5s weight with correct splitting & batch 64
#python train.py --img 640 --batch-size 64 --epochs 2000 --data DFG-tsd.yaml --weights '' --cfg 'yolov5s_200.yaml' --workers 10 --cache ram --device 0,1 --project Traffic_signs_v5s_scratch

# Start from scratch v5n weight with correct splitting & batch 64
#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights '' --cfg 'yolov5n_200.yaml' --workers 16 --cache ram --device 1 --project Traffic_signs_v5n_scratch

## Start from original v5x weight with correct splitting & batch 64
#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights yolov5x.pt --workers 16 --cache ram --device 1 --project Traffic_signs_v5x

# Start from scratch v5x weight with correct splitting & batch 64
#python train.py --img 640 --batch-size -1 --epochs 2000 --data DFG-tsd.yaml --weights '' --cfg 'yolov5x_200.yaml' --workers 16 --cache ram --device 1 --project Traffic_signs_v5x_scratch



# Start from scratch v5x weight with correct splitting & batch 64
python train.py --img 1280 --batch-size -1 --epochs 2000 --patience 500 --data DFG-tsd.yaml --weights Futes_A_Kis_Nebuloknak_Mert_Kertek/exp/weights/best.pt --workers 16 --cache ram --device 0,1 --project FutesAKisNebulokSzamara_2

