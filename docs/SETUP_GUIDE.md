# SmartPhotoVision - Setup Guide

## Features
| Feature | Description |
|---------|-------------|
| Face Detection | Automatic face detection in photos |
| Face Recognition | Identify known people across photos |
| Face Clustering | Group unknown faces into personas |
| Metadata Management | Extract and organize EXIF data |
| Smart Organization | Auto-sort photos by people, date, location |

## Prerequisites
- Python 3.8+
- OpenCV
- dlib (for face recognition)
- scikit-learn (for clustering)

## Installation
```bash
git clone https://github.com/shahidazam2020-oss/SmartPhotoVision-.git
cd SmartPhotoVision-
pip install -r requirements.txt
```

## Usage
```python
from smart_photo import PhotoManager

manager = PhotoManager("~/Photos")
manager.scan()           # Detect faces
manager.cluster()        # Group by person
manager.organize()       # Sort into folders
```

## Performance
| Photos | Processing Time |
|--------|----------------|
| 100 | ~30 seconds |
| 1,000 | ~5 minutes |
| 10,000 | ~45 minutes |