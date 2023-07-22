# FaceDetectionUsingFfmpegWithDlibInUnity
In a Unity environment, images streamed using FFmpeg are Mat-converted using OpenCV and face detection is performed by Dlib.

## Environmental Construction
1. Create a Unity project with a 3D template.
2. Window→Package Manager → Set "Packages" to "My Assets" in the upper left corner and import "OpenCV For Unity".
    <img src="/images/pack_01_openCV.png" width=680>
* Set up the system using the setup tool.

    <img src="/images/pack_01_openCV_setUp.png" width=480>


3. Import and setup Dlib Face Landmark Detector in the same way.

   <img src="/images/pack_01_Dlib_setUp.png" width=480>
4. Import and Setup [FFmpeg for Unity](https://assetstore.unity.com/packages/tools/video/ffmpeg-for-unity-199811).
5. Import [Runtime Inspector & Hierarchy](https://assetstore.unity.com/packages/tools/gui/runtime-inspector-hierarchy-111349).
6. Import [In-game Debug Console](https://assetstore.unity.com/packages/tools/gui/in-game-debug-console-68068#releases).
7. Import [FfmpegWithOpenCVForUnityExample.unitypackage](https://github.com/EnoxSoftware/FfmpegWithOpenCVForUnityExample/releases).
8. Rewrite the C# script named FfplayToMatHelperExample.cs in Assets/FfmpegWithOpenCVForUnityExample/FfplayToMatHelperExample/ (see diagram below) to the code named [FfPlayStreamingFaceDetectionExample.cs](/FfplayStreamingFaceDetectionExample.cs)

   <img src="/images/ProfectPath_FfplayToMatHelper.png" width=680>

By setting the URL appropriately, face detection can be performed from streaming video.
(However, we have confirmed that the delay is quite large.)

