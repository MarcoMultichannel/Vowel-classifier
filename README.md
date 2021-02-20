# Vowel-classifier
A simple classifier that uses the formants F1 and F2 to classify vowels. 
The dataset directory contains different audio files named accordingly, for instance "e (10).wav". 
For this case the vowels that got classified are the Italian ones. For each of the 7 vowels there are 20 .wav files.

Firstly, the audio files get normalized, then the formants get extracted using the parselmouth library. The values of F1 and F2 are taken 3 times within the audio, for a total of 6 features.
For giving a visual understanding of the data, the recorded vowels got plotted in a graph that has as axes the values of F1 and F2. The values used for plotting are the average of the 3 values taken.
The axes are inverted as to reassemble the form of the vowel trapezium.

Finally, the SVM model is created and tested. A logarithm transformation is used to improve performance and to make the graph look better.

![alt text](https://github.com/MarcoMultichannel/Vowel-classifier/blob/main/Graph.png)
