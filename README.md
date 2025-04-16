# Vehicle Damange Detection App

This app allows you upload a car image by simply dragging and dropping it. 
It will then analyze the image and tell you what kind of damage the car has.

For best results, use photos (Please use the sample photos provided in this repository)showing the car from a third-quarter front or rear view, as the model was trained on images from those angles
![app](app_screenshot.jpg)

### Model Details
1. Used ResNet50 for transfer learning
2. Model was trained on around 1700 images with 6 target classes
   1. Front Normal
   1. Front Crushed
   1. Front Breakage
   1. Rear Normal
   1. Rear Crushed
   1. Rear Breakage
9. The accuracy on the validation set was around 80%

### Set Up

1. To get started, first install the dependencies using:
    ```commandline
     pip install -r requirements.txt
    ```
   
2. Run the streamlit app:
   ```commandline
   streamlit run app.py
   ```
3. Upload a car image (third-quarter front/rear view) and see the prediction!