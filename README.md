# pyqtgui_yolo 250507
QT_designer를 이용해 만들어둔 프로그램을 yolov8을 사용하여 실시간 객체 인식이 되도록 만든 프로그램

# python패키지 설치
```
pip install requirements.txt
```
```
pip install ultralytics
```
# yolov5 > yolov8 새로 학습
기존 yolov5버전의 best.pt는 yolov8과 호환되지 않으므로 새로 학습해야함
(yolov5에서 쓰던 데이터셋은 호환 가능)
```
yolo task=detect mode=train data=dataset.yaml model=yolov8n.pt epochs=50 imgsz=640 device=0
```
# yolov5의 데이터셋을 가져온 후 경로 수정
![스크린샷 2025-05-07 180112](https://github.com/user-attachments/assets/838d915b-a5f9-400d-8333-99120caf3d6b)

# yolov8의 파일구조
![스크린샷 2025-05-07 175937](https://github.com/user-attachments/assets/99793bf9-3ee2-4cf6-a67c-98964dd40627)
# 실행 후 확인
![스크린샷 2025-05-07 174036](https://github.com/user-attachments/assets/201172d2-6318-4a00-b654-8c930d783694)


# 꼭 해야할 것 🙌
- PyTorch와 TorchVision 버전 맞춰주기
- GPU 작동 확인
- ![스크린샷 2025-05-07 180758](https://github.com/user-attachments/assets/feb47bf1-7d26-43cf-8bdb-cba6bc2bbc1d)
- yolov8 및 관련 라이브러리 설치하기
```
pip install ultralytics
pip install opencv-python
pip install PyQt6
pip install numpy==1.24.3
```
