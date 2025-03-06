# kidneystonedetction
Kidney Stone Detection using ResNet-18

This project provides a Flask-based web application to detect kidney stones using a trained ResNet-18 deep learning model. The model classifies medical images into four categories: Cyst, Normal, Stone, and Tumor.

Features
Upload medical images in .jpg, .png, etc. formats.
The ResNet-18 model makes predictions and returns the class along with the confidence score.
Supports GPU acceleration if CUDA is available.
Prerequisites
Python 3.x
Flask
PyTorch
Torchvision
Pillow (PIL)
Render templates like index.html
Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/kidney-stone-detection.git
cd kidney-stone-detection
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Place the kidney_stone_resnet18.pth model file in the project directory.

Usage
Start the Flask server:

bash
Copy
Edit
python app.py
Navigate to http://127.0.0.1:5000 in your browser.

Upload an image to receive the classification result with the confidence score.

Model
The model used in this project is ResNet-18, trained on a custom dataset to classify kidney images into the following categories:

Cyst
Normal
Stone
Tumor
API Endpoints
/: Home page for uploading images.
/predict: Accepts POST requests with an image file and returns the predicted class along with confidence.
Example
