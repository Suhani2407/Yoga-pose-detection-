# Yoga-pose-detection-
## Overview
This project uses AI to classify yoga poses and provide corrections. A pre-trained model extracts key points, which are analyzed by an MLP to identify the pose. It compares the test pose to an ideal pose and offers feedback for improvement, combining deep learning and computer vision.

## Features
- **Pose Recognition**: Identifies yoga poses from input images.
- **Ideal Pose Comparison**: Matches test poses to ideal poses using key points.
- **Corrective Feedback**: Provides detailed suggestions for pose improvement.

## Workflow
1. **Key Point Extraction**:
   - MediaPipe extracts key points from input images.
   - Key points are saved into a CSV file for further processing.

2. **Pose Classification**:
   - The CSV file is used as input to a trained Deep Learning model (MLP).
   - The model classifies the pose based on the extracted key points.

3. **Ideal Pose Dictionary**:
   - Ideal pose key points are stored in a dictionary using the same CSV data.
   - These key points act as a reference for comparison.

4. **Comparison and Feedback**:
   - Test pose key points are compared to the ideal pose key points.
   - Textual Feedback is generated to guide alignment and corrections.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/yoga-pose-detection-.git
   ```
2. Ensure MediaPipe and other dependencies are correctly installed.

## Usage
1. Run the script to process images and extract key points:
   ```bash
   jupyter notebook Yoga_pose.ipynb
   ```
2. Train the MLP model using the CSV file with key points and Test the pose and get feedback:
   ```bash
   jupyter notebook yoga-pose-detection-with-feedback.ipynb
   ```

## Technologies Used
- **MediaPipe**: For key point extraction.
- **Python**: Main programming language.
- **Deep Learning (MLP)**: For pose classification.
- **CSV Handling**: For data storage and processing.

## Results
The system classifies yoga poses with good accuracy and provides actionable feedback to help users align their poses with the ideal standard.

## Future Enhancements
- Add support for real-time pose correction.
- Enhance feedback with detailed visual guides.
- Expand the dataset to include more yoga poses.


## Contributors
- Suhani Thakur
