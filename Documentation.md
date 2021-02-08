# Raspberry-Pi-based-Reader-for-Blind
## Abstract:
It's quite difficult for visually impaired people to read a books, newspaper or any written document. 
Everytime they don't get braille to read everthing they want and it is costly also. So our device will give them opportuinity to read any thing at anytime they want. 
Our device is reading the text loud in form of audio as it captures image and all the text written there will be read out loud by the speakers. We have used OCR technology 
for converting the jpg image to text image and text image to audio by using TTS technology.

## Hardware Required:
1. Raspberry Pi 3B+
2. Raspberri Pi Camera
3. Flex Camera Connector 
4. Speaker
5. SD card
6. Led
7. Button
8. Resistance 220 ohm

## Language used:
1. Python 3

## Technology/Library used:
1. OCR Teachnology
2. TTS Technology (Text to Speech)

## About Components:
### 1. Raspberry Pi: 
   We are using 3B+ model of raspberry pi which has broadcom BC28837 SOC Cortex 7 Arm based Quadcore processor of speed.It is of 64 bit processor with speed of 1.4 GHz. 
   It can store data upto 1 GB SRAM and have a slot for SD card.
   It is having 40 GPIO pins, 4 USB and intregated wifi. It pins takes and gives output as 3.3V from its pins.
   #### For Installing OS in Raspberry Pi
For installing operating system, first we need to format the SD card then download and flash the raspbian software on it.Rasberry PI uses raspbian which is debian 
version of linux distributuion.
The os can be flased into the sd card using any 3rd party operating system like Etcher
### 2. Raspberry Pi Camera:
We are using raspberry Pi Camera as sensor which is 8 mega-pixel which have Sony IMX219 sensor. It have 3.68 X 2.76 and 4.66 mm diagonal
#### Interfacing of Raspberry Pi and Raspberri Pi Camera via Flex
![3099-02](https://user-images.githubusercontent.com/73650233/107179105-acb23500-69fb-11eb-8d5d-f774ff42e5ef.png)

## Block Diagram

![Colour Sensor – 2](https://user-images.githubusercontent.com/73650233/107228292-806dd700-6a42-11eb-86a2-a7ecfa6b007f.png)

## Circuit Diagram

![Colour Sensor – 1](https://user-images.githubusercontent.com/73650233/107228187-5f0ceb00-6a42-11eb-8d5c-ca2b75a5d058.png)

## Working 

Our device is used to convert the text file to sound. As we keep the document infront of the camera and it will capture the image. The image captures is send to the processor 
i.e. raspberry pi.The raspberry pi camera is connected with flux with the camera serial interface on raspberry pi.
When we press the button then it will start capturing the image and turn the led led on indicating processing has been started.
Now the image processing starts, first the document which is captured is in the png or jpg format which will get converted to grayscale and finally to txt format by using 
OCR technology.The converted text document is now using the TTS (Text to Speech) technology and converts the txt file into audioble format.
Then that signal is send to the the speaker/earphones via audio jack.
### OCR technology
OCR technology is the optical character recognition which converts the text document to the editable of searchable data with the use of pattern recognition and feature 
recognition.This technology is used so that we can edit, store search the data. In our case we are storing the data and converting into audio format.
 image captured --> image processing --> pre-processing --> segmentation (of lines and words) --> Recognition 
### TTS technology 
Text to speech technology is that technology which reads out loud the text to the audio. The ocr allows tts to convert the word on an image to readable format.
.txt file ---> processing (text to audio conversion) --> audio file

## Result
A visually impaired person can easily read any readable document using Raspberry Pi based Reader.
It will only capture image when we will press the button do processing and can hear what is written on those image.
