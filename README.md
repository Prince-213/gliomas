# Gliomas Detection with YOLOv11

A deep learning project that detects brain tumors in MRI images using a custom YOLOv11s model, deployed as an interactive Streamlit web application.

## Overview

This project implements a computer vision solution for medical image analysis, specifically designed to identify and localize brain tumors in MRI scans. The application uses a custom-trained YOLOv11s model to provide real-time detection with bounding box annotations directly in the web interface.

## Features

- 🧠 Upload MRI brain images in common formats (JPG, PNG)
- 🔍 Automatic tumor detection using YOLOv11s model
- 📊 Visual annotations with bounding boxes around detected tumors
- ⚡ Real-time processing and instant results
- 💻 User-friendly web interface built with Streamlit

## Project Structure

```
project/
├── streamlit_app.py      # Main Streamlit application
├── best.py              # Model loading and prediction functions
├── requirements.txt      # Python dependencies
├── packages.txt          # System dependencies for Streamlit Cloud
└── README.md
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Prince-213/gliomas.git
cd brain-tumor-detection
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Start the Streamlit application:
```bash
streamlit run streamlit_app.py
```

2. Open your web browser and navigate to `http://localhost:8501`

3. Upload an MRI image using the file uploader interface

4. View the processed image with tumor detection annotations

## Deployment on Streamlit Cloud

This app is configured for easy deployment on Streamlit Cloud:

1. Ensure all required files are in your GitHub repository:
   - streamlit_app.py
   - best.py
   - requirements.txt
   - packages.txt (if needed for system dependencies)

2. Connect your GitHub account to Streamlit Cloud

3. Deploy the app by selecting your repository and main file path (streamlit_app.py)

## Technical Details

- **Framework**: PyTorch
- **Model**: YOLOv11s custom architecture
- **Input Resolution**: 640×640 pixels
- **Supported Formats**: JPG, PNG

## Important Notes

- The `packages.txt` file ensures proper dependency resolution on Streamlit Cloud
- The `best.py` file contains the model loading and prediction logic
- Make sure your model weights are accessible to the application

## Limitations

- Performance may vary with image quality
- Not intended for clinical diagnosis without further validation

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Disclaimer**: This project is intended for research purposes only and should not be used for clinical diagnosis without proper validation and regulatory approval. Always consult healthcare professionals for medical advice.
