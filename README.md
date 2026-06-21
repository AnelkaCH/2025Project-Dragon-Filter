# Face Filter Dragon

A real-time animated face filter that places a dragon overlay on the user's face and animates it based on facial state — triggering fire or mouth animations when the user opens their mouth or eyes. Built on top of the Face Mesh module from the previous project.

## Overview

The program extends the `FaceMeshDetector` class with two new detection methods: `getSize()` to measure face region dimensions, and `isOpen()` to detect whether the mouth or eyes are open based on landmark distances. These states drive the filter animation — for example, the dragon "breathes fire" when the user's mouth opens. The dragon asset layers are composited onto the webcam feed each frame.

## Concepts Learned

- Extending an existing class with new methods (building on prior OOP work)
- Calculating distances between landmarks to infer facial state
- `isOpen()` logic using landmark ratio thresholds
- Animating overlay assets based on detected state
- `itertools` for cycling through animation frames
- Managing multiple overlay layers (base, mouth, eye animations)

## Demo

https://github.com/user-attachments/assets/8c5e38e8-7ab7-47ef-998b-174a5369ed54

## Setup

```
pip install mediapipe opencv-python numpy
```
