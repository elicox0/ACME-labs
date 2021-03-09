# facial-recognition

A Python class for identifying face images or, given a face image, finding the most similar image in the dataset. Currently only supports .jpg images that are 200x180 pixels.

## Usage
First, unzip the dataset faces94.zip into the same directory as facial_recognition.py. Alternatively, if you have a different dataset, copy it to
the same directory instead. Run the following in the same directory as the dataset and facial_recognition.py.

```python
from imageio import imread
import facial_recognition

data = FacialRec('Path_To_Dataset', m, n)

g = imread('Path_To_Face_To_Check')

data.find_nearest(g)
>>> 1 # Means that the face at index 1 is the closest face to g

data.match(g)
# Plots g along with the best match from the dataset
```

## Acknowledgement
This code began as the solutions to the Facial Recognition lab in Foundations of Applied Mathematics, Volume 1 
by Jeffrey Humpherys, Tyler J. Jarvis, and Emily J. Evans.
