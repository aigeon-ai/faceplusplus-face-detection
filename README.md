markdown
# Faceplusplus Face Detection MCP Server

## Overview

The Faceplusplus Face Detection MCP Server is designed to analyze and detect facial information from given images. This server provides advanced facial recognition capabilities, allowing users to extract detailed information such as face location, age, race, gender, and more from images. It's an ideal solution for applications requiring facial analysis and detection capabilities.

## Features

- **Face Detection**: Analyze the given image to detect facial information, including face location, age, race, gender, and more. This feature provides a comprehensive analysis of the face present in the image.

- **Face Landmark**: Obtain 1000 key points of the face from the uploaded image or a detected face token. This feature accurately locates facial features and contours, supporting dense facial landmark analysis for one face at a time. If multiple faces are present, it analyzes the one with the largest area. High-resolution images are recommended for optimal results.

## Tools

### Face Detection Tool

- **Description**: Detects facial information from the given image, including attributes such as face location, age, race, and gender.
- **Parameters**:
  - `image_url`: The URL of the image to be analyzed.
  - `return_attributes`: Comma-separated list of attributes to be returned, such as gender, age, smiling, headpose, facequality, blur, eyestatus, emotion, ethnicity, beauty, mouthstatus, eyegaze, skinstatus.

### Face Landmark Tool

- **Description**: Provides 1000 key points of the face, accurately locating facial features such as eyebrows, eyes, nose, mouth, and overall facial contours.
- **Parameters**:
  - `return_landmark`: Specifies which landmarks to return (e.g., left_eyebrow, right_eyebrow, left_eye, right_eye, nose, mouth, face). Default is all.
  - `image_url`: The URL of the image for landmark analysis.

## Usage Notes

- The server supports only one face at a time. If multiple faces are detected, it will analyze the face with the largest area. If areas are the same, a face is chosen randomly.
- For best results, use high-resolution images.

This MCP server is a powerful tool for applications needing precise and detailed facial analysis. With its ability to extract and analyze a wide range of facial attributes, it is suitable for various use cases, from security systems to user interaction enhancements.