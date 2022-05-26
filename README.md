https://github.com/karanjakhar/yolov5-export-to-raspberry-pi

git clone https://github.com/karanjakhar/yolov5-export-to-raspberry-pi.git
cd yolov5-export-to-raspberry-pi
chmod +x setup.sh
./setup.sh
python3 yolov5_tflite_folder_of_images_inference.py --weights yolov5s-fp16.tflite --folder_path images/ 
