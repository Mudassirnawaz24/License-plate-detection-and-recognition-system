

# 🚘 License Plate Detection and Recognition using OpenCV and Pytesseract

This project implements an automatic license plate detection and recognition system using Python. It leverages OpenCV for image processing and Pytesseract (Python wrapper for Tesseract OCR) for recognizing the alphanumeric text on license plates.

## 📸 Demo

![demo](samples/demo_result.png) <!-- Replace with your actual demo image path -->

## 🔍 Features

- License plate localization using edge detection and contour analysis
- Text recognition using Pytesseract
- Support for image or video input (e.g., webcam feed)
- Preprocessing techniques for noise reduction and contrast enhancement
- Real-time or batch processing of vehicle images

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- Pytesseract
- NumPy

## 📂 Project Structure

license-plate-recognition/
│
├── main.py # Main script to run detection and recognition
├── utils.py # Helper functions (preprocessing, plate detection, etc.)
├── samples/ # Sample images for testing
│ └── car1.jpg
├── output/ # Output folder for results (optional)
├── README.md # Project overview and instructions
└── requirements.txt # Required Python packages

ruby
Copy
Edit

## 🧪 Sample Results

Original Image               |  Detected Plate with OCR Text
:-------------------------:|:-------------------------:
![Input](samples/car1.jpg) | ![Result](samples/result_car1.png)

## ⚙️ Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/license-plate-recognition.git
   cd license-plate-recognition
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Install Tesseract-OCR

Windows: Download and install from here.

Linux:

bash
Copy
Edit
sudo apt-get install tesseract-ocr
Verify Installation

bash
Copy
Edit
tesseract --version
🚀 How to Run
To run detection and recognition on an image:

bash
Copy
Edit
python main.py --image samples/car1.jpg
To use webcam input (optional):

bash
Copy
Edit
python main.py --webcam
🧠 How It Works
Convert image to grayscale and apply filters

Detect edges using Canny edge detection

Find contours and identify license plate-like rectangles

Extract the region of interest (ROI) for the plate

Use Pytesseract to extract text from the plate region

Display or save the result

✅ Use Cases
Traffic monitoring systems

Smart parking systems

Toll booth automation

Vehicle access control

📌 Notes
OCR performance may vary with image quality and lighting.

Try different preprocessing options to improve recognition accuracy.

You can fine-tune Tesseract with language or configuration options.

📄 License
This project is open-source and available under the MIT License.
