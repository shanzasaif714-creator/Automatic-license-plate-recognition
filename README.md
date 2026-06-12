# Automatic License Plate Detection & OCR System (ALPR)

A real-time Automatic License Plate Recognition system using YOLOv11 for plate 
detection and EasyOCR for text extraction. Processes video streams frame-by-frame, 
draws bounding boxes, overlays recognized plate numbers, and exports annotated video.

## Results
- ✅ Precision: 0.99
- ✅ Recall: 0.955
- ✅ mAP50: 0.987
- ✅ Trained on 1,700+ images
- ✅ End-to-end video processing with annotated output

## Demo
▶️ [Watch Output Video on YouTube](https://www.youtube.com/watch?v=GxG3Z4BaOXk)

## Tech Stack
- Python
- Ultralytics YOLOv11
- EasyOCR
- Roboflow (dataset preparation)
- Google Colab
- OpenCV (video processing)

## Project Structure
- `plate_num_recognition` — YOLOv11 model training pipeline (Google Colab)
- `ocr_pipeline.py` — License plate OCR and video processing script (PyCharm)

## Model Weights
The trained model weights (`model.pt`) are not included in this repository due to file size.  
📩 Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/shanza-saif-704709357/) to request the model file.

## Dataset
Prepared and labeled using [Roboflow](https://roboflow.com). Contains 1,700+ labeled 
images of vehicle license plates.  
📦 [View Dataset on Roboflow](https://universe.roboflow.com/augmented-startups/vehicle-registration-plates-trudk)

## How to Run

### 1. Model Training (Google Colab)
1. Open `plate_num_recognition` in Google Colab
2. Connect to T4 GPU
3. Upload your dataset
4. Run all cells to train and export `model.pt`

### 2. OCR & Video Processing (Local)
1. Clone this repository
2. Install dependencies: `pip install ultralytics easyocr opencv-python`
3. Place your trained `model.pt` in the project folder
4. Run: `python ocr_pipeline.py`

## Notebook
- 📓 View on GitHub: `plate_num_recognition` (above)
- ▶️ Run in Colab: [Open in Google Colab](https://colab.research.google.com/drive/1n3deFNPLIwZpOyXpo4QlJsZzpoZcZML9?usp=sharing)
