# How to use project
Library used in project: dlib, face_recognition, imutils, requests <br /> <br />
First, create the following folders:
1. videos/
2. output/ <br />

Link video and output: https://drive.google.com/drive/folders/1aeVRMFLcSeHqiCU3bR_rbnjO4c0NDplE?usp=sharing <br />
You can add video for face recognition to videos/ <br /> <br />
Example how to run this project: <br />
Encoding faces
```bash
python encode_faces.py --dataset dataset --encodings encodings.pickle
```
Recognition in image
```bash
python recognize_faces_image.py --encodings encodings.pickle --image examples/example_01.png
```
Recognition in webcam <br />
A value of 1 displays and a value of 0 will not display the output frames to our screen.
```bash
python recognize_faces_webcam.py --encodings encodings.pickle --output output/jurassic_park_trailer_output.avi --display 1
```
Recognition in video
```bash
python recognize_faces_video.py --encodings encodings.pickle --input videos/lunch_scene.mp4 --output output/lunch_scene_output.avi --display 1
```
