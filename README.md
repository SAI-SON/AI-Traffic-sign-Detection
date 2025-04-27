# Traffic Signs Recognition

A real-time traffic sign recognition system using deep learning and computer vision. This project uses a convolutional neural network to classify different types of traffic signs through a webcam feed.

## Features

- Real-time traffic sign detection and recognition
- Support for 43 different traffic sign classes
- Live probability display for predictions
- Easy-to-use webcam interface

## Requirements

- Python 3.9 or higher
- Webcam
- Required packages (listed in requirements.txt)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/SAI-SON/AI-Traffic-sign-Detection.git
cd AI-traffic-signs-recognition
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Navigate to the Code directory:
```bash
cd Code
```

2. Run the recognition script:
```bash
python recognize.py
```

3. Point your webcam at a traffic sign
4. Press 'q' to quit the application

## Supported Traffic Signs

The system can recognize 43 different types of traffic signs, including:
- Speed limits (20km/h to 120km/h)
- No passing
- No entry
- Stop
- Yield
- Priority road
- And many more...

## Project Structure

```
AI-traffic-signs-recognition/
├── Code/
│   ├── recognize.py        # Main recognition script
│   ├── learn_signs.py      # Training script
│   ├── weights.h5          # Trained model weights
│   └── my_model/          # Model architecture
├── DataTraffic/           # Training data
├── requirements.txt       # Project dependencies
└── README.md             # This file
```

## Model Architecture

The CNN model consists of:
- Multiple convolutional layers with ReLU activation
- MaxPooling layers
- Dense layers with dropout for regularization
- Softmax output layer for 43 classes

## Performance

- Real-time processing at webcam frame rate
- Recognition threshold: 90% confidence
- Supports various lighting conditions

## Troubleshooting

1. If the camera doesn't initialize:
   - Try changing the camera index in recognize.py (e.g., from 0 to 1)
   - Check if your webcam is properly connected

2. If you get model loading errors:
   - Ensure all dependencies are correctly installed
   - Verify that the weights.h5 file is present in the Code directory

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- German Traffic Sign Recognition Benchmark (GTSRB) dataset
- TensorFlow and Keras teams
- OpenCV community 