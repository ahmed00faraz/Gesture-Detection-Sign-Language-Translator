# Hand Gesture Data Collection with MediaPipe and OpenCV

This project captures hand gesture data using OpenCV and MediaPipe. It organizes motion frames for various gestures and exports keypoints in `.npy` format for training gesture recognition models. The project includes user-friendly countdowns to ensure smooth and accurate data collection.

## Features
- Gesture detection using MediaPipe's holistic model.
- Systematic data organization for training.
- Countdown timers for precise data collection.
- Easy customization for different gestures and dataset sizes.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/hand-gesture-collection.git
   cd hand-gesture-collection
   ```

2. Install dependencies:
   ```bash
   pip install opencv-python mediapipe numpy
   ```

3. Ensure you have a working webcam.

## Usage

1. Define your gestures and dataset parameters in the script:
   ```python
   actions = ["wave", "thumbs_up", "peace"]
   no_sequences = 30  # Number of samples per gesture
   sequence_length = 30  # Frames per sample
   ```

2. Run the script:
   ```bash
   python gesture_data_collection.py
   ```

3. Follow on-screen instructions for countdowns and gesture collection.

4. Data will be saved in the `MP_Data` directory, organized by gesture and sample sequence.

## Directory Structure
The captured data is stored as follows:
```
MP_Data/
|-- wave/
|   |-- 0/
|   |   |-- 0.npy
|   |   ...
|-- thumbs_up/
|-- peace/
```

## Dependencies
- Python 3.7+
- OpenCV
- MediaPipe
- NumPy
- Tensorflow
