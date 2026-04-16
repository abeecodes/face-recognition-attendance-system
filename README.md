# Face Recognition Attendance System

This project implements a face recognition-based attendance system using a single Google Colab notebook. It automatically detects and recognizes faces and records attendance using computer vision techniques.

---

## Overview

The system provides a streamlined pipeline within a Colab notebook to:

* Detect faces from video frames
* Generate and store facial encodings
* Match detected faces with known identities
* Record attendance with timestamps in an Excel file

The entire implementation is contained within one notebook for simplicity and ease of execution.

---

## Technologies Used

* Python
* OpenCV
* Face Recognition Library
* NumPy
* OpenPyXL
* Google Colab

---

## Dependencies

Install the required libraries using:

```
!pip install face_recognition
!pip install opencv-contrib-python
!pip install openpyxl
```

---

## Libraries Used

```python
import cv2
import face_recognition
import os
import pickle
import numpy as np
import openpyxl
from openpyxl.styles import PatternFill, Font, Alignment
from datetime import datetime
from google.colab.patches import cv2_imshow
```

---

## How It Works

1. Face images are loaded from a dataset directory
2. Facial encodings are generated and stored for known individuals
3. Input frames are captured and processed
4. Detected faces are matched against stored encodings
5. Attendance is recorded in an Excel file with date and time

---

## How to Run

1. Open the notebook:

   ```
   FACE_RECOG_SYSTEM.ipynb
   ```

2. Run the installation cells to install dependencies

3. Execute all cells sequentially

4. Ensure dataset paths are correctly configured in the notebook

---

## Notes

* The project is implemented entirely within a single Colab notebook
* Dataset, trained models, and additional files are not included in this repository
* File paths may need to be updated based on your environment

---

## Future Improvements

* Add dataset and model management
* Improve user interface and usability
* Integrate real-time camera input
* Add analytics and reporting features
