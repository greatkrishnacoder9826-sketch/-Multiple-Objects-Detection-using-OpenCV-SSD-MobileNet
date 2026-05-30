🚗 Multiple Objects Detection using OpenCV & SSD MobileNet

A real-time Multiple Object Detection project built with OpenCV DNN and the SSD MobileNet v3 COCO model. This project can detect and classify multiple objects in images, videos, and live webcam feeds.

📌 Features
Detect multiple objects in a single frame
Real-time object detection using webcam
Video file object detection support
Bounding box visualization
Object class labeling
Uses pre-trained COCO dataset model
Fast and lightweight SSD MobileNet architecture
🛠️ Technologies Used
Python
OpenCV
SSD MobileNet v3
COCO Dataset
Matplotlib
📂 Project Structure
Multiple-Objects-Detection/
│
├── frozen_inference_graph.pb
├── ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt
├── person.txt
├── object_detection.ipynb
├── images/
├── videos/
└── README.md
📥 Installation
1. Clone the Repository
git clone https://github.com/your-username/Multiple-Objects-Detection.git
cd Multiple-Objects-Detection
2. Install Required Libraries
pip install opencv-python matplotlib numpy
📦 Required Model Files

Download the following files:

frozen_inference_graph.pb
ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt

These files are part of the TensorFlow SSD MobileNet model.

🚀 Usage
Image Detection
img = cv2.imread("image.jpg")
ClassIndex, confidence, bbox = model.detect(img, confThreshold=0.5)
Video Detection
cap = cv2.VideoCapture("video.mp4")
Webcam Detection
cap = cv2.VideoCapture(0)
⚙️ Model Configuration
model.setInputSize(320,320)
model.setInputScale(1.0/127.5)
model.setInputMean((127.5,127.5,127.5))
model.setInputSwapRB(True)
🎯 Detectable Objects

The model is trained on the COCO dataset and can detect 80+ object classes, including:

Person
Car
Bicycle
Motorcycle
Bus
Truck
Dog
Cat
Chair
Laptop
Bottle
Traffic Light

and many more.

📸 Output Example

The model draws:

✅ Bounding Boxes
✅ Object Labels
✅ Confidence-based Detection

Example:

Person
Car
Dog
Bicycle

detected simultaneously in a single frame.

🔮 Future Improvements
Object Tracking
Distance Estimation
Counting Objects
Face Detection Integration
YOLOv8 Implementation
GPU Acceleration
👨‍💻 Author

Krishna Great

Python & Computer Vision Enthusiast

⭐ Support

If you found this project useful:

Star the repository ⭐
Fork the repository 🍴
Share with others 🚀
📜 License

This project is open-source and available under the MIT License.
