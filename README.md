# License Plate Detection with Transfer Learning

## Overview
This project builds a **License Plate Detection system** using **Transfer Learning** and applies **EasyOCR** to extract license numbers.  
It can be used in **automatic parking management systems**.

The dataset used is the [License Plate Dataset on Kaggle](https://www.kaggle.com/code/sayamkumar/car-license-plate-detection).

---

## Tech Stack
- Python, TensorFlow, Keras
- EasyOCR
- Transfer Learning (MobileNet, RetinaNet50)
- TensorFlow.js (TFJS) & TensorFlow Lite (TFLite) for deployment

---

## Features
- Detects license plates in images using **object detection models** (MobileNet, RetinaNet50)  
- Two transfer learning approaches:
  1. Fine-tune the entire pre-trained model  
  2. Few-shot training for classification and bounding box detection  
- Applies **EasyOCR** to read license numbers  
- Regular expressions applied to validate **Algerian license plate format** (e.g., first part contains 5 or 6 digits)  
- Model exported to **TFJS** and **TFLite** for web and mobile deployment  

---

## Usage

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/license-plate-detection.git
cd license-plate-detection
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run detection on images
```bash
python detect_license_plate.py --image path/to/image.jpg
```

### 4. Optional: Run OCR extraction
```bash
python extract_plate_number.py --image path/to/image.jpg
```

## Results
- Model trained on Kaggle dataset and evaluated successfully
- Tested on Algerian license plates with high accuracy after applying regex rules
- Model works for both detection and OCR recognition of license numbers

---

## Deployment
- Exported model versions:
  - **TFJS** for web applications
  - **TFLite** for mobile or embedded devices

---

## Future Improvements
- Extend OCR support for multiple countries’ license plate formats
- Integrate with real-time video streams for automatic parking systems
- Improve detection accuracy with more diverse datasets

---

## Impact
This project provides a complete end-to-end solution for license plate detection and recognition, suitable for **parking management, security systems, and vehicle tracking applications**.
