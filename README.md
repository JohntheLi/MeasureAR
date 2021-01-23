# MeasureAR
Simple measurement application using AR Foundation and Unity. Tested on Android devices using ARCore, should work on iOS through ARKit as well.

You can measure custom AR objects:
![alt text](https://imgur.com/a/Xevz9gH)

Or real-life objects:
![alt text](https://imgur.com/a/7jNYaql)


## Requirements:
- ARCore supported Android device
- Unity (Unity Hub can be used to install JDK/Android SDKs for you)
- An EchoAR account (https://www.echoar.xyz/) for real-time object modification, or you can use a standard static object if desired.

## Installation Instructions:
1. In Unity Hub, go to the 'Projects' tab and select 'ADD'.
2. Select the project directory.
3. Ensure that Unity, AR Foundation, ARCore, and Android SDKs are set up according to the QuickStart Guide (https://developers.google.com/ar/develop/unity-arf/quickstart-android).
4. Select the EchoAR prefab object, and input your custom key in the field that says <YOUR_API_KEY_HERE> under 'Inspection'.
5. If you choose not to use an EchoAR object, you can instead drag your own prefab into the 'Placed Prefab' field under 'Place on Plane' script in AR Origin object.
6. Connect your Android Device to the computer via USB cable.
7. Select 'Build and Run' to run the application on your phone.

## Usage Instructions:
The app has two modes:
1. Object Placement mode, which allows you to place an EchoAR object on any plane
2. Measurement Tape mode, which allows you to drag your finger between any two points on a plane to create a measurement.

- You can easily switch between modes by clicking on their respective buttons in the UI. 
- Note that because both modes depend on plane detection, it may take a few seconds to move your camera around before the plane you are trying to measure may register.
- If the placed Object is too large, you can modify the scale of the object in the EchoAR console (see https://docs.echoar.xyz/unity/transforming-content)
