# Federated Learning for Multimodal Stress Detection

This project implements a privacy-preserving Federated Learning (FL) framework for human stress detection using video, audio, and ECG modalities. Each client trains locally on its device, and only model weights are shared with the server, ensuring maximum privacy and secure distributed training.

##  Features
- Uses multimodal encoders: Video CNN, Audio Dense Network, and ECG 1D-CNN.
- Implements Federated Learning with FedAvg for secure distributed training.
- Supports local client-side training without sharing raw data.
- Central server handles global model aggregation and updates.
- Automatically generates Accuracy, Loss, and Smoothed IEEE-style plots.
- Privacy-focused architecture — video, audio, and ECG signals never leave the device.
- Modular design for easy replacement of encoders.
- Scalable and supports multiple clients.
- Round-wise logging and visualization.

##  Project Abstract
Stress detection systems usually require centralizing sensitive biometric data, raising privacy and security concerns. This project proposes a Federated Learning–based multimodal stress detection system, enabling distributed on-device model training. Raw data remains local, while only model updates are shared.

##  Installation & Setup
### 1. Clone
`git clone https://github.com/adeshankush058/Fedfusion_Federated-Learning_project.git`

### 2. Create Virtual Environment
`python -m venv venv`

### 3. Install Dependencies
`pip install -r requirements.txt`

##  Usage
### data perprocessing 
`data_preprocessing.ipymb`

### Start model traning
`fl_model_traning.ipynb`

### Start model traning for 50 
`fl_50round.ipynb`



##  Model Architecture
Video CNN, Audio Dense, ECG 1D-CNN → Fusion Network.

## Federated Workflow
Initialize → Train locally → Send weights → FedAvg → Update → Repeat.

##  Outputs
Accuracy (20 & 50 rounds), Loss curve, Smoothed accuracy.

## Privacy
No raw data leaves clients.

##  Datasets
Stress-Id,FER2013,RAVDESS.

##  Limitations
Requires multiple clients, depends on dataset quality.

##  Future Enhancements
Secure aggregation, differential privacy, mobile deployment, dashboards.

##  Team
Adesh, Tushar


