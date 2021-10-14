# iot_turtleProject-openpose
python-openpose determines whether user's neck is bended or not
사진을 분석하여 사용자의 목 각도를 측정하는 모듈


# reference
- 사용자의 허리 각도를 구하는 소스 참고
(https://hanryang1125.tistory.com/6)

- openpose github repo 
(https://github.com/CMU-Perceptual-Computing-Lab/openpose)

# Installation
1. Download zip file
2. Go to [openpose-master](https://github.com/CMU-Perceptual-Computing-Lab/openpose) and download zip file.
3. In that file, model installation command 
for Mac
```
cd openpose-master
./models/getModels.sh
```
for Windows
```
./models/getModels.bat
```
4. If installation is done, copy files `models/pose/mpi/pose_iter_160000.caffemodel` and `models/pose/mpi/pose_deploy_linevec_faster_4_stages.prototxt`
5. put those files in same directory that `main.py` exists.
6. put one or more image files in the same directory, and correct image files' name in `main.py` code.
7. start command:
```
python3 main.py
```
