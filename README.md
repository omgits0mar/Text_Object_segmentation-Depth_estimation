# Object Detection and Depth Estimation for the Visually Impaired

This project aims to assist visually impaired individuals in taking photos and searching for specific objects within them. It does this by using a combination of OpenAI's ClipSeg zero-shot object segmentation and a depth estimation model.

## Overview

1. A user takes a photo with their device.
2. The user's voice is recorded and transcribed into a text prompt.
3. The text prompt is used as input to the ClipSeg model to identify specific objects within the photo.
4. The objects identified by ClipSeg are then used to mask the original photo and apply a depth estimation model to the masked portion of the photo.
5. The model outputs whether the object is near or far using thresholding.
6. The output is then converted to speech for the visually impaired user to hear.

## Requirements

Python 3
OpenAI's ClipSeg
Intel DPT depth estimation model
Voice recognition system (e.g. Google Cloud Speech-to-Text API)
Text-to-speech library (e.g. Google Text-to-Speech API)

## Example

Here's an example of how the project can be used:

1. A visually impaired individual wants to find a specific book in a library.
2. They take a photo of the bookshelf and record themselves saying "find the book titled 'The Great Gatsby'."
3. The photo and voice prompt are passed through the object detection and depth estimation models.
4. The output is read aloud to the individual: "The book titled 'The Great Gatsby' is found and close."

## Note :

This repo and code feature is an open source python notebook part of the graduation project App `Smart Vision for Visually impaired` which aims to help visually impaired people sense and know what is going around by using AI, Computer Vision and Deeplearning to create powerfull features in a mobile app that could help those everyone in needs
This App is currently in developing of some features as :
1. Optical characater recognition (OCR) for reading text in many languages.
2. Friends face recognition using Siamese one-shot learn
3. Currency detection (Egyptian banknotes ✅) using YOLO object detection and EGYPT-IRIS dataset.
4. Image Caption and Scene Recognition of surroundings usind Pre-trained large models.
5. Voice commands (Trigger words detection) for choosing which feature the patiant wants by voice in the application
6. **Object detection filtered by text and depth estimating the distance of this object using OpenAi's ClipSeg and Intel's DPT models**.
Though in this notebook doesnot feature the text to speech output or speech extraction to command prompt as these are used in the app only.

## Acknowledgments

- ClipSeg model from OpenAI
- DPT model from Intel
- Example code for using ClipSeg and DPT in Python
