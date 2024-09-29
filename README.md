# Handpose_Estimation

This project implements a **3D hand pose recognition** system using a dataset of hand joint coordinates. It includes visualizations of hand keypoints in 3D space and a nearest-neighbor matching algorithm to identify similar hand poses based on normalized keypoints.

## Features

- **3D Hand Pose Visualization**: Displays 3D hand keypoints and bone connections using Matplotlib.
- **Keypoint Normalization**: Normalizes hand poses by centering on the palm and scaling for consistency.
- **Nearest-Neighbor Matching**: Finds the closest matching hand pose from a dataset using a custom Euclidean distance-based loss function.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/marwanthestudent/Handpose.git
    ```

2. **Install dependencies**:
   Ensure you have Python installed. Install the required libraries:
    ```bash
    pip install numpy scipy matplotlib
    ```

3. **Dataset**:
   Unzip and Place the dataset files (`train_joint_data.mat`, `test_joint_data.mat`) in the `hand_pose_data` directory.

## Usage

1. **Run the project**:
    ```bash
    python main.py
    ```

2. **Key functionalities**:
   - Visualize a hand pose from the dataset in 3D.
   - Normalize hand keypoints based on the palm keypoint.
   - Find and display the closest matching hand pose using nearest-neighbor search.

## Example Output

An example of a 3D visualization with two different hand poses is shown below:

![image](https://github.com/user-attachments/assets/22614cf6-67af-4fc1-b311-8a5852e63752)


## Future Work

- Improve the performance of the nearest-neighbor algorithm by incorporating a KD-Tree for faster searches.
- Implement advanced pose estimation techniques using deep learning.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
