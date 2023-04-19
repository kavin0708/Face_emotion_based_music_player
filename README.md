# face-emotion-based-music-player
Face Emotion based music player is a novel approach that helps the user to automatically play songs according to the emotions of the user
Music Player using Fase Emotion Recognition

This is a project based on the concept of Computer Vision and Emotion detection. In this project, I have used computer vision to detect the emotion a person is exhibiting. Through the emotion detected, the system shall identify a song playlist according to the mood of the user.
It will provide an easy access to any song the user wants to listen according to his/her mood thus decreasing the work of switching to apps for the particular songs. 
The project is based on the technology of Computer Vision and specifically on the subfield of Emotion detection. 
This technology is used in coordination with the generation of desired music based on the mood detected. This project diminishes the need for switching in between various music apps. 

As the technology is advance every second, humans, nowadays tend to be drawn towards smart work rather than hard work. And nowadays, music has become an essential part of every individual's life. So, incorporated these two prevailing factors and created this project.

Libraries used:
1. Cv2 
2. Sys 
3. Pandas 
4. Random 
5. Datetime 
6. Numpy 
7. Tensorflow 

Flow (Layman Language):
* Train model using retrain.py(see 'how to train.txt'). It Creates a model file retrain.pb
* run label.py
It detects the face using cv2(OpenCV) using haarcascade
* provide the face image to label_image.py -> returns the detected emotion(in integer 1/2/3/4) using trained model file. 
Store emotions 10 times.
* check the emotion with highest count -> map the integer to the correct emotion(as defined in dictionary)
* Provide the emotion to play_music_pygame.py -> under '/emotions file' check for the corresponding csv.
* Read any random song name from the csv -> Play the corresponding song from '/songs'
Show necessary logs on the command prompt.
