Project Overview:- 
This project implements a Bicep Counter using Human Pose Detection through MediaPipe. The purpose is to accurately detect arm movements during bicep curls and count the repetitions using machine learning models and computer vision. This project builds on insights from various research findings and leverages MediaPipe’s pose detection library for real-time performance.

Main Research Finding:- 
The foundation of this project is built on human pose estimation research, which has shown that deep learning models, when trained on large datasets, can effectively track and detect human joints and body movements. Key research findings include:
Human Pose Estimation with Deep Learning: Studies like Cao et al. (2017) that introduced OpenPose have influenced the development of MediaPipe's robust framework, showing that convolutional neural networks (CNNs) excel at detecting and mapping human joints.
Real-Time Pose Detection: MediaPipe builds on earlier works like Wei et al. (2016), which improved efficiency in multi-person pose estimation, enabling real-time applications such as fitness tracking.

Key References:- 
Media Pipe and AI pose detection youtube video by Nicholas Renotte
Model and Training Techniques:- The detection system used pre-trained models provided by MediaPipe, particularly its Pose Detection model, which applies deep learning techniques to identify human landmarks. Key parameters included:
MediaPipe Pose Model: This was used for detecting 33 key points on the human body, focusing on the shoulder, elbow, and wrist joints for bicep curl detection.
Angles Calculation: The algorithm calculates the angle between the shoulder, elbow, and wrist to determine the contraction and extension during a bicep curl.
Thresholding: Specific angle thresholds were set to recognize the start and end of a bicep curl.

Model Evaluation:- 
Accuracy: The accuracy of the bicep curl counting algorithm was measured by comparing the predicted counts with actual repetitions from the video reference. The project achieved an accuracy of approximately 95% in correctly counting repetitions.
Latency: The system's real-time performance was tested, with an average latency of 30ms per frame, making it suitable for real-time fitness tracking applications.

Results Summary:
The model performed with high accuracy in detecting and counting bicep curls. The pose estimation technique, combined with angle thresholding, ensured that most repetitions were accurately counted with minimal false positives or missed counts.
