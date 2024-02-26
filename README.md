# Sign-Language-Recognition
The project aims to develop a real-time sign language detection system. It utilizes mediapipe library, computer vision and a deep learning model (LSTM) to detect and recognize hand gestures in real-time video streams.

## Technologies and Tools
* Python
* TensorFlow
* MediaPipe
* OpenCV

## Components
### Data Collection: 
The dataset includes 10 actions: hello, thankyou, yes, no, help, great, please, sorry, iloveyou, and goodbye.  
Each action was recorded in 30 separate video sequences, with each sequence comprising 30 frames captured at a consistent frame rate.

### Keypoint Extraction with MediaPipe Holistic:
MediaPipe Holistic is used to detect and extract keypoints representing various body landmarks, including hand gestures and facial expressions from input video frames.

### Data Preprocessing and Feature Extraction:
Feature Vector Creation: These extracted keypoints were processed to create feature vectors.
Labeling: Feature vectors were labeled according to the corresponding sign language action, creating labeled datasets for training and testing the LSTM model.

### LSTM Model Training:
The LSTM model architecture was designed to accept sequences of keypoints as input and predict the corresponding sign language action.  
The model was evaluated using metrics such as accuracy_score and confusion_matrix.

### Real-Time Sign Language Detection:
Once trained and evaluated, the LSTM model was deployed for real-time sign language detection.  
Keypoints were continuously extracted from video frames using MediaPipe Holistic, fed into the trained model for prediction, and the recognized sign language actions were displayed in real-time.

### Screenshots of some actions

![ily](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/acded46e-ccdb-4965-9616-bf8850423832 )  

![help](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/7be144e0-e00c-43a8-9a75-fe08d2940bc5)  

![great](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/b3df6f26-2138-404a-8d55-e89cb1726cee)

![hello](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/00feec64-421c-45e2-88fd-5e2fe1448deb)

![please](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/067e6614-73cd-458f-93a7-3b8ee0fd101c)

![no](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/631b1e40-de12-4c40-a8ba-3872ea7abfe2)


![goodbye](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/d5c6ce5c-aa62-4bf2-b1bc-14b5e850ac3c)


![thankyou](https://github.com/Quisha16/Sign-Language-Recognition/assets/90545228/196947ea-4f03-4ec8-9d1e-9bb558a87ec0)




