# Deeptector
##### - Real Time Action Classification Project
  
#### 1. 프로젝트 설명
#### 2. 개발 환경 구축 및 설치
#### 3. 특징
#### 4. 사용법
#### 5. Demo
  
## 1. 프로젝트 설명
Deeptector는 Openpose를 통해 사람의 Feature를 뽑아낸 후 해당 데이터를 통하여 사람의 행동을 분류하는 프로젝트입니다. 본 프로젝트는 Feature의 추출 과정과 그 데이터를 뉴럴 네트워크를 통해 학습시킨 간단한 모델을 기본으로 제공합니다. 사용자는 데이터를 다른 방법으로 전처리하고 새로운 모델을 만들어 사용할 수 있습니다.
  
또한 본 프로젝트는 Darknet 및 Openpose, Tensorflow와 같은 라이브러리를 GPU를 이용하여 사용하고 있습니다.
[![Watch the video](https://img.youtube.com/vi/FrkhI3JcsXE/0.jpg)](https://www.youtube.com/watch?v=FrkhI3JcsXE)

위 사진을 클릭하여 동영상을 확인할 수 있습니다.
  
  
## 2. 개발 환경 구축 및 설치
#### 2-1 개발 환경
  - 개발 OS는 Ubuntu 16.04 환경에서 진행되었습니다.
  
  
#### 2-2 사전 설치 프로그램
  - [1. Nvidia Driver 및 Cuda, Cudnn](https://github.com/Deeptector/Deeptector/blob/master/document/cuda.md)
  - [2. OpenCV 3.4.0](https://github.com/Deeptector/Deeptector/blob/master/document/opencv.md)
  - [3. Python 및 Tensorflow](https://github.com/Deeptector/Deeptector/blob/master/document/tensorflow.md)
  - [4. Darknet](https://github.com/Deeptector/Deeptector/blob/master/document/darknet.md)
  
위 링크를 통하여 1, 2, 3, 4번 순서로 설치를 진행합니다.
  
  
#### 2-3 Deeptector 설치
Git으로 부터 해당 프로젝트를 다운받고 해당 프로젝트 폴더로 이동합니다.
```sh
$ git clone https://github.com/Deeptector/Deeptector.git
$ cd Deeptector
```
  
Makefile을 만들기 위해 편집기를 이용하여 deeptector.pro 파일을 수정합니다.
```sh
$ vi deeptector.pro
```
vi 편집기 화면이 갱신되면 <username>을 사용자 username으로 변경합니다.
```sh
:%s/<username>/사용자username
```
다른 편집기의 사용도 가능합니다. deeptector.pro 파일의 <username>을 사용자의 username으로 변경합니다.
  
수정이 완료되었다면 Makefile을 생성하기 위하여 다음 명령어를 입력합니다.
```sh
~/Deeptector$ sudo qmake
```
2-2 과정을 통해 OpenCV 설치를 진행하셨다면 sudo 명령어를 필수로 입력해야 합니다. (sudo 미입력 시 OpenCV 라이브러리를 가져오지 못할 수 있습니다.) 

생성된 Makefile을 통하여 빌드를 진행합니다.
```sh
~/Deeptector$ make
```
  
  
## 3. 특징
  
  
## 4. 사용법
  
  