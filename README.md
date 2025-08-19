# Real-Time-Intelligent-Traffic-Monitoring-and-Control-System 🚦👥�🚗

[![Python 3.7+](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.8-green)](https://opencv.org/)
[![YOLOv8](https://img.shields.io/badge/YOLO-v8n-red)](https://ultralytics.com/yolov8)

Real-time AI-powered traffic management system combining computer vision and IoT for adaptive signal control.

![System Demo](screenshots/demo.gif) *Add actual screenshot of the GUI here*

## Key Features ✨
- **Dual Object Detection**  
  👥 Pedestrians (YOLOv8 class 0)  
  🚗 Vehicles (Cars, Bikes, Buses, Trucks - classes 2,3,5,7)
- **Adaptive Traffic Logic**  
  ⚖️ Priority given to pedestrians when:  
  `(ped_count ≥ vehicle_count) OR (vehicle_count == 0)`
- **Live Feed Display**  
  🖼️ Dual-stream GUI with real-time annotations and counters
- **Hardware Integration**  
  🚦 Arduino/Raspberry Pi traffic light control via serial
- **Performance Optimized**  
  ⚡ Frame skipping (3:1 ratio)  
  📊 5-frame moving average smoothing
- **Interactive Controls**  
  🎮 Keyboard commands for detection toggle and shutdown

## Installation 🛠️

### Requirements
- Python 3.7+
- Webcam (USB or built-in)
- (Optional) Arduino with traffic light LEDs

```bash
# Clone repository
https://github.com/DinithaNipunaka/Real-Time-Intelligent-Traffic-Monitoring-and-Control-System

# Install dependencies
pip install ultralytics opencv-python pyserial

# Download pretrained YOLOv8n model (auto-downloaded if missing)
wget https://github.com/ultralytics/assets/releases/download/v8.1.0/yolov8n.pt 
```
## Run the Project:
pip install notebook
jupyter notebook
pip install pyserial
pip install scikit-learn

## Keyboard Controls:
- q: Quit system
- d: Toggle detection on/off
## Contribution
Contributions are welcome! If you'd like to improve the system or fix a bug, please fork the repository and submit a pull request.
## License 📄
Distributed under the MIT License. See LICENSE for more information.
