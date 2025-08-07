# Sign-Language-Detector

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- Required Python packages (listed in `requirements.txt`) such as OpenCV, MediaPipe, NumPy, etc.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/1rishu0/Sign-Language-Detector.git
    cd Sign-Language-Detector
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Usage Workflow

1. **Collect Data**  
   Run `collect_imgs.py` to capture hand gestures via webcam. Label and save landmark data to build your dataset.

2. **Create Dataset**  
   Use `create_dataset.py` to preprocess raw data, generating a structured `.pickle` dataset ready for training.

3. **Train the Model**  
   Execute `train_classifier.py` to train a classifier (likely using scikit-learn) on the prepared dataset. This script outputs a serialized `model.p` file.

4. **Inference / Real-Time Detection**  
   Launch `inference_classifier.py` to perform live gesture recognition using your webcam and the trained model.

### Demo

https://github.com/user-attachments/assets/93ad1bac-1be3-41c8-a810-ea1ee849557d

## License

This project is released under the **GPL‑3.0 License**, so feel free to modify and share as per the license terms. :contentReference[oaicite:0]{index=0}

## Contributing

Contributions are welcome! Here’s how you can help:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your work and push to your fork.
5. Open a Pull Request with details of your enhancements.
