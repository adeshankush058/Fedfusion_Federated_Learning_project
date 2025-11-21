# Fedfusion_Federated-Learning_project
This project implements a privacy-preserving Federated Learning system for detecting human
stress using video, audio, and ECG data. Each client trains locally and only shares model
updates with the server, ensuring no raw data leaves the device.

#Features

1)The system uses multimodal encoders, including a Video CNN for facial expression analysis, an Audio Dense Network for MFCC-based voice stress detection, and an 
ECG 1D-CNN for physiological signal extraction.
2)It implements a full Federated Learning workflow with FedAvg aggregation to combine client models without sharing raw data.
3)Each user device performs local training on its private dataset, ensuring data never leaves the client.
4)The server performs a global model update after aggregating client weights and distributes the improved model back to all clients.
5)The framework automatically generates accuracy plots, loss curves, and smoothed IEEE-style graphs for performance evaluation.
6)The entire system is built around a privacy-first architecture, preventing any exposure of video, audio, or ECG data to external servers.
7)The design supports scalable multi-client participation, allowing more users to join training without system modification.
8)The project includes modular code, making it easy to replace encoders, modify aggregation strategies, or experiment with new fusion techniques.
9)Training logs and visualizations provide round-wise performance tracking, useful for research and debugging.

# run the requirement.txt to ger the proper lib you need 










































