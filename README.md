# RECOG: Object Recognizer App

<img src="https://i.ibb.co/fDn57tx/Screenshot-2024-01-26-at-11-52-01-PM.png">

This project consists of making an Android application that automatically captures pictures, names the objects, and gives their location. This app is intended to help visually impaired people so that they can know what is in front of them by just opening the app. Our UI is made in a way that the user doesn’t need to take pictures. The app itself is going to take pictures and analyze them every couple of seconds by default.

## How it works:

The application operates by capturing images at regular intervals, typically every few seconds. Each image is converted into a Base64 encoded format, representing binary data in an ASCII string format. This encoded image is subsequently transmitted to a dedicated server for further processing.

Upon receiving the image, the server decodes it from its Base64 format to its original form. The decoded image is then temporarily stored on the server. During this phase, the server applies various enhancement techniques to the image. These enhancements include adjusting the image's color, contrast, and sharpness. The objective of these modifications is to accentuate the details of individual objects within the image, making them more distinct and easier to recognize.

Following the enhancement process, the server sends the improved image to the Google Cloud Vision API. This API is a powerful tool provided by Google that utilizes machine learning to analyze and interpret the content of images. The API processes the enhanced image and provides a response that includes information about the elements identified within the image.

Finally, the server converts this information into a descriptive string. This string is designed to concisely and accurately convey the contents of the image. The server then sends this string back to the application. Once received by the app, the string is read aloud to the user. This feature is particularly beneficial for individuals who may have visual impairments, as it provides an auditory representation of the visual information captured by the app.

<p align="center">
<a href="https://ibb.co/Xs4YNnJ"><img src="https://i.ibb.co/7Wzk83y/Screenshot-2024-01-26-at-11-58-58-PM.png" alt="Screenshot-2024-01-26-at-11-58-58-PM" border="0"></a>
</p>

## How to Build:
1. Go to the `misc` folder
2. Download the APK, and install the app on your phone
3. After installation, open the app; everything should work perfectly.

<i>Note: This app can only be used on an Android smartphone that has a functioning camera</i>

---
[Demo Video](https://www.youtube.com/watch?v=xvoobCyBV2U)

We appreciate your interest in our app. There will be updates soon!
<!--  -->