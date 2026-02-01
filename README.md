# 🎥 Video Feature Extraction Tool

A Python-based tool that analyzes a local video file and extracts key visual and temporal features using computer vision techniques.
Built as part of the Machine Learning Engineer task for White Panda.

# 📂 Project Structure
├── video_feature_extractor.py

├── sample_video.mp4

├── README.md

# 🚀 Features

The tool extracts the following features from a video:

✅ Shot Cut Detection

Detects hard cuts (abrupt scene changes)

Uses grayscale histogram comparison

Outputs total number of detected cuts

✅ Motion Analysis

Computes average motion using Farneback Optical Flow

Measures frame-to-frame movement magnitude

✅ Text Detection (OCR)

Uses Tesseract OCR

Samples frames at fixed intervals

Calculates the ratio of frames containing readable text

# 📥 Input

Path to a local video file (.mp4, .avi, etc.)

Example:

video_path = "sample_video.mp4"

# 📤 Output

The extracted features are returned as a dictionary and printed in JSON format.

Example output:

{
    "video_path": "sample_video.mp4",
    "shot_cut_count": 4,
    "average_motion": 1.12,
    "text_present_ratio": 0.0
}
