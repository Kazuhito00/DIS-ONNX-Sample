# DIS-ONNX-Sample
背景除去モデルである[DIS/IS-Net](https://github.com/xuebinqin/DIS)のPythonでのONNX推論サンプルです。<br>
変換自体を試したい方は、Google Colaboratory上で[Convert2ONNX.ipynb](Convert2ONNX.ipynb)を使用ください。<br>

![image](https://user-images.githubusercontent.com/37477845/221350125-de577e58-dc1c-4dc2-80ed-4dd253cfeacf.png)

# Requirement 
* OpenCV 4.5.3.56 or later
* onnxruntime 1.8.0 or later
* gdown 4.6.4 or later ※「model/isnet-general-use.onnx」ファイルが無い場合

# Demo
デモの実行方法は以下です。
```bash
python demo_DIS_onnx.py
```
* --device<br>
カメラデバイス番号の指定<br>
デフォルト：0
* --movie<br>
動画ファイルの指定 ※指定時はカメラデバイスより優先<br>
デフォルト：指定なし
* --model<br>
ロードするモデルの格納パス<br>
デフォルト：model/isnet-general-use.onnx
* --score_th<br>
マスク値の閾値 ※指定する場合は0.5など小数値を指定<br>
デフォルト：None

# Reference
* [xuebinqin/DIS](https://github.com/xuebinqin/DIS)

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)
 
# License 
DIS-ONNX-Sample is under [Apache 2.0 License](LICENSE).
