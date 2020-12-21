# Mask_YOLO
---
### Reference

1. YOLO Fine Tuning, https://medium.com/analytics-vidhya/covid-19-face-mask-detection-using-yolov5-8687e5942c81

1. YOLO dataset, https://github.com/iAmEthanMai/mask-detection-dataset.git

1. YOLOv5 Code, https://github.com/ultralytics/yolov5
---
### Execution

Basic Exmaple

저희가 fine tuning한 weight는 weights 폴더 안에 best.pt로 저장되어 있습니다.

웹캠을 통해 detection을 실행하실려면 source argument를 0으로, 다른 사진이나 동영상에 detection을 실행하려면 DATA_PATH를 입력하시면 됩니다.

    python detect.py --weights ./weights/best.pt --conf 0.4 --source 0
    
    python detect.py --weights ./weights/best.pt --conf 0.4 --source DATA_PATH
