# happymimi_bringup
## Overview
happymimi_bringupはhappymimiの基本機能を開始するためのroslaunchスクリプトを起動します。

## Description
このパッケージには、2つのlaunchファイルがあります。
### minimal.launch
ロボットベースに設置されたマイコンと通信を開始します。

### sensor.launch
下記センサーの起動を行います。
- UTM-30LX (2D-LiDAR)
- RealSense Depth Camera D435i (RGB-D Camera)
- ReSpeaker Mic Array v2.0 (Microphone Array)
- Dynamixel Motor (Servo Motor)

## Usage
minimal.launchの起動

`roslaunch happymimi_bringup minimal.launch`

sensor.launchの起動

`roslaunch happymimi_bringup sensor.launch`

オプションで起動するセンサーを指定できます。

`roslaunch happymimi_bringup sensor.launch realsense=false respeaker=false`
