python detect.py --weights test_runs/model/best.pt --source 'test_runs/data' --data data.yaml 


### Converting to ONNX

Use onnx = 1.12.0

pip install onnx==1.12.0

And export the model with opset version 12, not the default 17.


python export_mod.py --weights test_runs/model/best.pt --opset 12 --include onnx 

Onnx conversion issue: https://github.com/ultralytics/yolov5/issues/10665 



Model visualisation: https://netron.app/

