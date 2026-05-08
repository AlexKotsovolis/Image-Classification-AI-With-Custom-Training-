# 🧠 Custom Image Classifier

A modern desktop application for training and running your own custom image classification model using **PyTorch**, **ResNet-18**, and **Tkinter**.

This project lets you:

- Create custom classes dynamically
- Train a lightweight neural network head on top of a pretrained ResNet backbone
- Classify single images or entire folders
- Monitor training progress with a modern GUI
- Build your own personalized image recognition system with minimal setup

---

## ✨ Features

- 🎯 Transfer Learning using pretrained ResNet-18
- 🖼️ Single image classification
- 📁 Batch folder classification
- 🧪 Dynamic custom class creation
- ⚡ Fast feature extraction
- 📊 Live training logs + progress tracking
- 🎨 Modern dark-themed Tkinter interface
- 💾 Automatic model + metadata saving
- 🔁 Real-time prediction previews

---

# 📸 Preview

<img width="1084" height="896" alt="image" src="https://github.com/user-attachments/assets/47a03442-09c9-4873-9c6b-5a2d7500e8a5" />



preview/
├── app-ui.png
├── training.png
└── classification-results.png
🏗️ Project Structure
.
├── images/                     # Default folder for image classification
├── custom_classes/             # User training datasets
│   ├── cats/
│   ├── dogs/
│   └── cars/
│
├── custom_head.pth             # Saved classifier head
├── custom_classes.json         # Saved class metadata
├── main.py                     # Main application
└── README.md

⚙️ Installation
1. Clone the Repository
git clone https://github.com/yourusername/custom-image-classifier.git
cd custom-image-classifier
2. Install Dependencies
pip install torch torchvision pillow
▶️ Running the App
python main.py
🧠 How It Works

This project uses Transfer Learning.

Instead of training an entire CNN from scratch:

A pretrained ResNet-18 acts as a frozen feature extractor
A custom classification head (nn.Linear) is trained on your own classes
The model learns quickly even with small datasets
Pipeline
Input Image
   ↓
Image Preprocessing
   ↓
ResNet-18 Feature Extraction
   ↓
Custom Linear Head
   ↓
Prediction + Confidence Score
🏋️ Training Your Own Classes
Step 1 — Add a Class

Click:

+ Add Class

Then:

Enter a class name
Select a folder containing training images

Example:

cats/
dogs/
cars/
Step 2 — Train

Click:

Train

The app will:

Extract image features
Train the classification head
Save the trained weights automatically
🔍 Classification
Single Image
Browse for an image
Click Classify

The app returns:

Prediction: Cat (98.2%)
Folder Classification

Select a folder containing images and classify them all at once.

Useful for:

Dataset sorting
Automated labeling
Bulk image organization
🧪 Data Augmentation

Training includes:

Random crops
Horizontal flips
Color jitter

This improves generalization and model robustness.

🛠️ Tech Stack
Technology	Purpose
PyTorch	Deep Learning
TorchVision	Pretrained models + transforms
Tkinter	Desktop GUI
Pillow	Image processing
ResNet-18	Feature extraction backbone
📈 Future Improvements
 GPU / CUDA support
 Drag-and-drop image support
 Export predictions to CSV
 Confusion matrix visualization
 Dataset balancing tools
 ONNX export
 Multi-threaded training
 Better checkpoint management

🧹 Model Persistence

The application automatically saves:

custom_head.pth
custom_classes.json

So your trained classes persist between sessions.

⚠️ Notes
Minimum recommended:
20–50 images per class
Better lighting and image variety improves accuracy
At least 2 classes are required before training
🧑‍💻 Author

Built with caffeine, PyTorch, and questionable sleep schedules.

📜 License

MIT License

Feel free to use, modify, and distribute this project.

⭐ Support

If you like this project:

Star the repo
Fork it
Improve it
Break it
Train it on memes
