# How to use project
First, create the following folders:
1. videos/
2. output/
You can add video for face recognition to videos/
Example how to run this project
Encoding faces
```bash
python encode_faces.py --dataset dataset --encodings encodings.pickle
```
recognition in image
```bash
python recognize_faces_image.py --encodings encodings.pickle --image examples/example_01.png
```
recognition in webcam
```bash
python recognize_faces_webcam.py --encodings encodings.pickle --output output/jurassic_park_trailer_output.avi --display 1
```
recognition in video
```bash
python recognize_faces_video.py --encodings encodings.pickle --input videos/lunch_scene.mp4 --output output/lunch_scene_output.avi --display 1
```
