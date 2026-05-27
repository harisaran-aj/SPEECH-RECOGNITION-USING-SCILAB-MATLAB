# EXP 5 : SPEECH RECOGNITION USING SCILAB

## AIM: 
To perform and verify speech recognition using SCILAB. 

## APPARATUS REQUIRED: 
PC with Google Colab

## PROGRAM : 
```
import speech_recognition as sr

r = sr.Recognizer()
r.energy_threshold = 100
r.dynamic_energy_threshold = True

# Use the actual uploaded file path
audio_file = "WATT.wav"

with sr.AudioFile(audio_file) as src:
    print("Processing...")
    audio = r.record(src)

try:
    text = r.recognize_google(audio, language="en-IN")
    print("Recognized Text:", text)
except Exception as e:
    print("Error:", e)
```
## OUTPUT: 
<img width="924" height="537" alt="image" src="https://github.com/user-attachments/assets/f58a83f8-f046-4582-acf6-2e0b9c626edc" />


## RESULT: 
Thus the speech recognition using Python was performed and verified.
