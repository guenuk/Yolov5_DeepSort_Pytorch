python3 -m venv venv   
. venv/bin/activate  
pip install -r requirements.txt 
git clone --recurse-submodules https://github.com/mikel-brostrom/Yolov5_DeepSort_Pytorch.git
python track.py --yolo_model yolov5/models/best.pt --source yolov5/src/testVideo.mp4 --save-vid
