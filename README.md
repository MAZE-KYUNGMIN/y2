https://github.com/karanjakhar/yolov5-export-to-raspberry-pi

git clone https://github.com/karanjakhar/yolov5-export-to-raspberry-pi.git
cd yolov5-export-to-raspberry-pi
chmod +x setup.sh
./setup.sh
python3 yolov5_tflite_folder_of_images_inference.py --weights yolov5s-fp16.tflite --folder_path images/ 


```

counter, fps = 0, 0
fps_avg_frame_count = 10
start_time = time.time()
  
  
    if counter % fps_avg_frame_count == 0:
      end_time = time.time()
      fps = fps_avg_frame_count / (end_time - start_time)
      start_time = time.time()

    # Show the FPS
    fps_text = 'FPS = {:.1f}'.format(fps)
    text_location = (left_margin, row_size)
    cv2.putText(image, fps_text, text_location, cv2.FONT_HERSHEY_PLAIN,
                font_size, text_color, font_thickness)
```
