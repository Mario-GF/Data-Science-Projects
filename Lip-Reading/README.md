# LipReading

  *lip reading web application designed to accurately decipher spoken words from video footage*. Built upon the powerful LipNet model, this application employs advanced deep learning techniques to analyze and interpret lip movements with remarkable precision.


![Screenshot 2024-04-10 020423](E:\work\LipReading\image.png)



### Dataset 
The dataset used for training the model is a subset of the [Grid Corpus Dataset](https://spandh.dcs.shef.ac.uk//gridcorpus/) .
Used ```gdown``` to download a subset (1 speaker) of the full dataset (34 speakers) from google drive.

To Download complete dataset please run the following line of code in your terminal:
```
bash GridCorpus-Downloader.sh FirstSpeaker SecondSpeaker
```
where FirstSpeaker and SecondSpeaker are integers for the number of speakers to download

> NOTE: Speaker 21 is missing from the GRID Corpus dataset due to technical issues.

### Tech Stack Used
1. Python-Tensorflow-Keras -> data preparation, pipeline, model training & testing.
2. Streamlit -> web application.
3. LipNet -> lip reading model architecture idea.
4. ffmpeg -> video file format conversion
6. opencv -> video capture and frames processing.

### Note: Further Scope
Implementing dlib for video processing to include all types of videos, including live video input.

### References
1. [LipNet: End-to-End Sentence-level Lipreading - Yannis M. Assael, Brendan Shillingford, Shimon Whiteson, Nando de Freitas](https://arxiv.org/abs/1611.01599)
2. [Sequence Modelling with Connectionist Temporal Classification(CTC), an algorithm used to train deep neural networks in speech recognition, handwriting recognition and other sequence problems.](https://distill.pub/2017/ctc/)
3. [LipNet: End-to-End Sentence-level Lipreading - GitHub Code implementation](https://github.com/rizkiarm/LipNet)
4. [Keras Automatic Speech Recognition With CTC](https://keras.io/examples/audio/ctc_asr/)





