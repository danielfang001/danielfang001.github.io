---
layout: post
Title: Final Project Daily Log
---

Below is a log of my daily progress, including:

1.) What I worked on today

2.) What I learned

3.) Any road blocks or questions that I need to get answered

4.) What my goals are for tomorrow

**January 7th**
I basically reviewed materials and other people's work on music generation using LSTM and music21 for MIDI data extraction. I learned about the difference between STM and LSTM, having additional forget and output update function. I still need to explore the actual code for LSTM, and I will work on this particularly with Eric. My Goal for tomorrow is that I'm able to start inputing the data preproccessed.

**January 8th**
Today, without Eric's presence in class, I learned about the ways to make our code run faster. SInce our last run took 5 hours, we need to find a server GPU that can save us time. I looked mainly at google colab and google cloud platform. I tried google colab and realized that it is very hard to upload the dataset directly from local. I'm going to try to upload our huge data set( >10GB) to github and access through github from colab. I also started reading about the other people's example of using LSTM to read midi files that are converted into matrixes. I still need to work out how the model works because there are a lot of layers. My goals for tomorrow is to build our own model and learn more about the example's model before that.

<img src="/images/code.png" width="350"/> 

**January 9th**
Today, I read about the code that I posted yesterday. We used his code as the basic structure of our model. However, with his model and his parameters, the accuracy is very low (1% to 5%). We have two theories to improve. The first is that we need to change the model and optimize the model parameters. The second is to change the way we preprocessed the data.  We have already finished the text version of the midi model and got a reasonable result, and now we're trying to convert the midi file into a matrix, which has a lot of ways to achieve. In our original preprocessing, we have values in the same column ranging from 0 to 1, and we are going to try to one hot the dataset to improve the accuracy. In addition, we will continue to look at how other people transform the midi file and how they use LSTM. Tomorrow, I will take my day off, so I will see what Eric worked on and add my own work during weekend.
dataValid.close() 

**January 10th**
Wellness Day

**January 13th**
Today, I worked on researching the third way of preprocessing out data, which is to use the sound waveform of the music and transform it somehow to plug it into LSTM. I read a paper who directly inputs the audio but doesn't necessarily explain how they process the data so it becomes a matrix/vector. I found another example using GANs, which is a way to analyze parameters of the tone. However, result is the same piece of music with different tone, but we want actually different piece of music that the computer composes. Then I read about another paper, which explained that they used Fourier transformation to process the original audio file into frequency representations.  They claimed that they were attempting to avoid and disregard the natural inclusion of music theories if they consider the specific notes and pitches, which the midi method provides. Tomorrow, I will need to try it with our own data, Fourier transformation (also different kinds of FTTs) is built-in in numpy so I can test it out right away tomorrow. 
**January 15th**

**January 16th**

**January 17th**