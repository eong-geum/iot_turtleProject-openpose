# iot_turtleProject-openpose
python-openpose determines whether user's neck is bended or not


# reference
https://hanryang1125.tistory.com/6
https://github.com/CMU-Perceptual-Computing-Lab/openpose

# Installation
1. Download zip file
2. Go to openpose_github(https://github.com/CMU-Perceptual-Computing-Lab/openpose) and download zip file.
3. In that file, model installation command for Mac
```
./models/getModels.sh
```
, for Windows
```
./models/getModels.bat
```
4. If installation is done, copy files `models/pose/mpi/pose_iter_160000.caffemodel` and `models/pose/mpi/pose_deploy_linevec_faster_4_stages.prototxt`.
5. put those files in same directory with `main.py`.
6. put one or more image files in the same directory, and set correct image files on `main.py`
7. start command:
```
python3 main.py
```
