# Speech-to-Sign-language-Translator
**An application which takes in live speech or audio recording as input, converts it into text and displays the relevant Indian Sign Language images or GIFs.**
- Front-end using EasyGui.
- Speech as input through microphone using PyAudio. 
- Speech recognition using Google Speech API and Sphix(for offline use).
- Text Preprocessing using NLP.
- Dictionary based Machine Translation.

## To run the application.
1. Open the Downloads folder and then open the terminal.
2. From the terminal, run the *main* python file using the command **python main.py**.
3. The application interface appears on the screen.
4. Hit the record button to start taking speech as input.
5. Any speech recorded is then processed and respective outputs are shown accordingly.
6. To exit the application using speech, say *goodbye*.


**Sign language is a visual language that is used by deaf people as their mother tongue. Unlike acoustically conveyed sound patterns, sign language uses body language and manual communication to fluidly convey the thoughts of a person. Due to considerable time required in learning the Sign Language,  it becomes difficult to communicate with these specially abled people, and thus creates a communication gap.**

## Objective
**This Audio to Sign Language converter aims at :**
- Providing information access and services to deaf people in Indian sign language.
- Developing a scalable project which can be extended to capture whole vocabulary of ISL through manual and non-manual signs

It can be developed as a desktop or mobile application to enable specially abled people to communicate easily and effectively with others

## Algorithm
Audio to Sign Language Translator
1. Start
2. Getting the Speech
   1. Listen for 1 second and calibrate the energy threshold for ambient noise
levels.
   2. Listen the Speech using Microphone.
Now the energy threshold is already set to a good value, and we can
reliably catch speech right away.
3. Recognise the Speech.
4. Convert Speech to Text.
   1. Make the Text to lowercase for further manipulation.
5. Detected Text
   1. If “goodbye” then exit.
   2.Else if Detected Text in predefined Dictionary Words. Display
respective GIFs of the Phrase.
   3. Else Count the Letters of the Word/Phrase.
      1. Display the Visual of the phrase with some delay of Actions.
   4. Continue all the steps from Step 3, and continue till the Speech Ends.
6. If Error in Step 2, That is if no Speech Detected then display error message
“Could not listen”.









# <h2>Sign Language to Speech Conversion </h2>

<div align= "center">
  <h4>Sign Language to Speech Conversion system built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to communicate using Indian Sign Language(ISL) based gestures in real-time video streams with differently abled. </h4>
</div>











## TechStack/framework used

- [OpenCV](https://opencv.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)


## Data Distribution
The dataset used can be downloaded here - [Click to Download](https://drive.google.com/drive/folders/16ce6Hc4U5Qr6YBArcozoYom6TT5-7oSc?usp=sharing)

This dataset consists of __17113 images__ belonging to 27 classes:
*	__Training Set: 12845 images__<br />



## Features
The model is capable of predicting gestures from Indian sign language in real-time with high efficiency. These __predicted alphabets__ are converted to form __words__ and hence forms __sentences__. These sentences are converted into __voice modules__ by incorporating __Google Text to Speech__(gTTS API).</br></br>
The model is efficient, since we used a compact __CNN-based architecture__, it’s also computationally efficient and thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.). This system can therefore be used in real-time applications which aims at bridging the the gap in the process of communication between the __Deaf and Dumb people with rest of the world__.

## Feature Extraction
* Gaussian filter is used as a pre-processing technique to make the image smooth and eliminate all the irrelevat noise.
* Intensity is analyzed and Non-Maximum suppression is implemented to remove false edges.
* For a better pre-processed image data, double thresholding is implemented to consider only the strong edges in the images.
* All the weak edges are finally removed and only the strong edges are consdered for the further phases. <br />





















