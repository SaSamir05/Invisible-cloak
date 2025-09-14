# Invisible-cloak ⏰

# Invisible Cloak - Python Project

A magical **invisibility cloak** built using **Python** and **OpenCV**. This project leverages **real-time video processing** to make an object of a specific color (like a red cloak) appear invisible by replacing it with the background.

## Features

* Real-time invisibility effect using a webcam.
* Color detection using **HSV color space**.
* Smooth masking with morphological operations for realistic output.
* Background replacement for creating a magical invisibility effect.

## How It Works

1. **Capture Background:**
   The program first captures the background image without the cloak. This background will later replace the color of the cloak.

2. **Color Detection:**
   The cloak’s color is detected in HSV color space. Here, we use **red** as an example, but it can be changed to any color by adjusting the HSV ranges.

3. **Masking & Morphology:**
   A mask is created for the cloak color, cleaned using **morphological operations** (open and dilate) to remove noise.

4. **Background Replacement:**
   The cloak area is replaced with the background, while other parts of the frame remain unchanged, creating a convincing invisibility effect.

## Installation

1. Make sure you have **Python 3.x** installed.
2. Install dependencies:

   ```bash
   pip install opencv-python numpy
   ```

## Usage

1. Run the script to capture the background:

   ```bash
   python capture_background.py
   ```

   Press **'q'** to save the background.

2. Run the main invisibility script:

   ```bash
   python invisible_cloak.py
   ```

   Press **'q'** to quit.

3. Enjoy your **invisibility cloak** in real-time!

## Customization

* You can change the cloak color by adjusting the **HSV ranges** in the script.
* Adjust **morphology iterations** to improve mask quality.
* Use any webcam or video source supported by OpenCV.

## Requirements

* Python 3.x
* OpenCV
* NumPy
* Webcam

