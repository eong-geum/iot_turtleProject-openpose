# iot_turtleProject-openpose

python-openpose determines whether user's neck is bended or not <br>
사진을 분석하여 사용자의 목 각도를 측정하는 모듈

사진에 보이는 사용자의 옆모습에서, <br>
목 아래 부터 귀까지의 직선이 얼마나 기울어졌는지 측정하여 거북목을 판단한다.

# demo results

<img width="430" alt="스크린샷 2021-10-15 오후 5 15 46" src="https://user-images.githubusercontent.com/43146778/137455138-262b8f69-9dbb-4a9e-b55e-4a5a8253be7c.png">
<img width="417" alt="스크린샷 2021-10-15 오후 5 15 57" src="https://user-images.githubusercontent.com/43146778/137455321-eb217f09-5bca-428d-9a87-be60c0e2efac.png">

# reference

- 사용자의 허리 각도를 구하는 소스 참고 <br>
  (https://hanryang1125.tistory.com/6)

- openpose github repo <br>
  (https://github.com/CMU-Perceptual-Computing-Lab/openpose)

- demo image source <br>
  (https://news.nate.com/view/20190906n05074?mid=n0400)

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

4. When installation is done, copy files `models/pose/body_25/pose_deploy.prototxt` and `models/pose/body_25/pose_iter_584000.caffemodel`
5. put those files in same directory that `main.py` exists.
6. put one or more image files in the same directory, and correct image files' name in `main.py` code.
7. install opencv-python

```
pip install opencv-python
```

8. start command:

```
python3 main.py
```
