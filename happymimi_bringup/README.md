# happymimi_bringup
## Overview
happymimi_bringupは、happymimiの基本機能を開始するためのroslaunchスクリプトを起動します。

## Description

### minimal.launch
- ロボットベース制御ボードの起動

- ロボットモデルの生成

> [happymimi_description]()にあるxacroファイルを読み込んで、ロボットモデルを生成します。

- パラメータの生成
 > [happymimi_params]()にあるyamlファイルを読み込んで、ROSパラメータを生成します。

### sensor.launch
下記センサーの起動を行います。
- UTM-30LX (2D-LiDAR)
- RealSense Depth Camera D435i (RGB-D Camera)
- ReSpeaker Mic Array v2.0 (Microphone Array)
- Dynamixel Motor (Servo Motor)

## Usage
### minimal.launchの起動

`roslaunch happymimi_bringup minimal.launch`

### sensor.launchの起動
全てのセンサを起動する時は、下記コマンドを端末に入力してください。

`roslaunch happymimi_bringup sensor.launch`

オプションで起動するセンサーを指定できます（デフォルトでは全てtrue）。

`roslaunch happymimi_bringup sensor.launch realsense=false respeaker=false`
