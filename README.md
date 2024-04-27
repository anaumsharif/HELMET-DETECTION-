## Helmet Detection Using YOLOv7

This project focuses on helmet detection using YOLOv7, a state-of-the-art deep learning object detection model. The goal is to detect helmets in images or video streams, providing a solution for safety and compliance applications in various industries. This README provides an overview of the project, its features, usage instructions, and examples.
The "Helmet Detection Using YOLOv7" project employs the YOLOv7  deep learning model for detecting helmets in images or video streams. This project is designed to enhance safety and compliance in various industries by automatically identifying individuals wearing helmets in real-time scenarios.

Key Components and Functionality:
YOLOv7 Model:
Utilizes the YOLOv7 object detection model, which is an advanced variant of the YOLO (You Only Look Once) architecture.
Offers a good balance between detection accuracy and inference speed, making it suitable for real-time applications.
### Features

- **Helmet Detection**:
  - Utilizes YOLOv7 for robust and accurate detection of helmets.
  - Supports real-time detection in video streams or batch processing of images.

- **Object Localization**:
  - Identifies the location (bounding box) of helmets within the input data.
  - Provides confidence scores for detected helmet instances.

### Prerequisites

Before running the scripts, ensure you have the following installed:

- Python (version 3.x recommended)
- PyTorch (installation instructions [here](https://pytorch.org/get-started/locally/))
- OpenCV library (`opencv-python`)
- YOLOv7 implementation (e.g., from [Ultralytics YOLOv5 GitHub](https://github.com/ultralytics/yolov5))

Install the required libraries using pip:

```bash
pip install torch torchvision opencv-python
```

### Usage

1. **Clone YOLOv7 Repository**:

   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   ```

2. **Navigate to YOLOv7 Directory**:

   ```bash
   cd yolov5
   ```

3. **Run Helmet Detection Script**:

   ```bash
   python detect.py --source input_image.jpg --weights yolov5s.pt --conf 0.5 --img-size 640
   ```

   Replace `input_image.jpg` with the path to your input image or video.

### Scripts Overview

- **`detect.py`**:
  - Main script for performing helmet detection using YOLOv7.
  - Loads the specified input image or video and runs object detection to identify helmets.

### Examples

#### 1. Helmet Detection in an Image

```bash
python detect.py --source input_image.jpg --weights yolov5s.pt --conf 0.5 --img-size 640
```

![Helmet Detection in Image](path/to/image_result.jpg)

#### 2. Helmet Detection in a Video

```bash
python detect.py --source input_video.mp4 --weights yolov5s.pt --conf 0.5 --img-size 640
```

### Contributing

Contributions are welcome! If you have ideas for improvements, bug fixes, or additional features, feel free to fork the YOLOv7 repository and submit a pull request.

### License

This project is based on the YOLOv7 implementation, which is open-source and distributed under the [MIT License](https://github.com/ultralytics/yolov5/blob/master/LICENSE).

### Next Steps

Explore the YOLOv7 documentation and experiment with different model configurations (`yolov5s.pt`, `yolov5m.pt`, `yolov5l.pt`, `yolov5x.pt`) for varying levels of detection accuracy and speed. Customize the detection pipeline to suit specific use cases involving helmet detection, and integrate additional functionalities as needed.

---

This project leverages the power of YOLOv7 for helmet detection tasks, offering a versatile and efficient solution for safety applications. Use it to enhance workplace safety, streamline compliance processes, or explore the capabilities of deep learning-based object detection. If you have any questions or feedback, please engage with the YOLOv7 community or contribute to the development of this project. Happy helmet detecting!
