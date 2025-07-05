# 📦 Barcode & QR Code Detection
---
A real-time computer vision project designed to detect and decode barcodes and QR codes using Python and OpenCV. The system captures live video from a camera, processes each frame to enhance features, and identifies encoded data. It provides immediate visual feedback by highlighting detected codes with polygons, making it a practical solution for retail, inventory management, logistics, and other scanning applications.

---

## 📋 Input Overview

This project uses a live camera feed as the input source to detect barcodes and QR codes in real time.

* **Input:** Frames captured from the webcam (or any camera device).
* **Outputs:** Decoded data printed to the console and annotated frames displaying detected regions.

---

## 🚀 Features

* **Real-Time Detection:** Continuously processes camera frames to detect QR codes and barcodes.
* **Decoding:** Extracts data from detected codes and prints it instantly.
* **Visual Feedback:** Marks detected codes with green polygons for easy identification.
* **Robust Preprocessing:** Uses edge detection, sharpening, adaptive thresholding, and histogram equalization to improve detection accuracy.
* **Interactive:** Runs until the user presses `'a'` to exit.

---

## 🛠️ Tools and Libraries

* **Programming Language:** Python
* **Computer Vision:** OpenCV
* **Numerical Computing:** NumPy
* **Development Environment:** Jupyter Notebook, VS Code, or any Python IDE

---

## 📈 Methodology

1. **Frame Capture:** Opens the default camera using OpenCV’s `VideoCapture`.
2. **Preprocessing:**

   * Applies vertical edge detection and sharpening.
   * Converts to grayscale, applies Gaussian blur and adaptive thresholding.
   * Enhances contrast using CLAHE.
3. **Detection & Decoding:**

   * Uses `cv2.QRCodeDetector` to detect and decode QR codes.
   * Uses `cv2.barcode_BarcodeDetector` to detect and decode multiple barcodes.
4. **Visualization:**

   * Draws green polygons around detected QR codes and barcodes.
   * Displays the annotated video in a real-time window.
5. **Termination:**

   * Continues running until the user presses `'a'` to quit.

---

## 🎯 Usage

### Clone the repository:

```bash
git clone https://github.com/abdelrahman-abozarifa04/Barcode-QR-Detection.git
cd Barcode-QR-Detection
```

### Install dependencies:

```bash
pip install opencv-python numpy
```

### Run the project:

```bash
python main.py
```

---

## 📊 Results

* **Detection:** Accurately identifies QR codes and barcodes in real-time.
* **Decoding:** Prints decoded text (like URLs or numeric codes) to the console.
* **Visualization:** Highlights detected codes with green outlines for user-friendly feedback.

Example Outputs:

```
QR Code Detected: https://example.com
Barcode Detected: 123456789012
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo, open issues, or submit pull requests.

---

## 📧 Contact

**Abdelrahman Abozarifa**

* GitHub: [@abdelrahman-abozarifa04](https://github.com/abdelrahman-abozarifa04)
* Email: [as0144549@gmail.com](mailto:as0144549@gmail.com)

---

## ⭐ Acknowledgements

Thanks to the open-source community for providing powerful tools like OpenCV that make real-time computer vision applications accessible.

---

✅ If you’d like, I can also generate:

* A `requirements.txt`
* A `.gitignore`
* Or a sample GIF/demo badge for your README.

Just tell me what you want! 🚀
