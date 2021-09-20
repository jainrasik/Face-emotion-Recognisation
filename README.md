# Realtime Face Emotion Recognisation 


## Authors

- [@Rasik Jain](https://www.github.com/Jainrasik)

  
## Documentation

  ### Abstract: 
Face emotion recognisation is detecting the   emotion of human via using some AI, computer vision and deep learning alogrithms. This emotion detection serves various used cases  in industries be it in education, robotics, automobile and other industries. In this project       the data set for training the model is obtained from hidor kirill dropbox folder. For emotion    classification, we divide the images into seven classes  i.e. angry, disgust, fear, happy, neutral, sad, and surprise. We will use transfer        learning and obtained pre trained weights for our model from the mobilenetv2. First data       set loaded and converted it into the input          format of mobilenetv2. We then remove the output layer and add our own output layer       having 7 outputs correspond to number of       classes present in our dataset. Then we use         realtime web feed image which can be                 obtained via using streamlit webrtc library into our model and obtained the prediction.       Finally we build web app using streamlit and       deploy the model in amazon aws EC2 instance so that it can be access across world wide          web.
### Problem Statement
The Indian education landscape has been undergoing rapid changes for the past 10 years owing to the advancement of web-based learning services, specifically, eLearning platforms.
Global E-learning is estimated to witness an 8X over the next 5 years to reach USD 2B in 2021. India is expected to grow with a CAGR of 44% crossing the 10M users mark in 2021. Although the market is growing on a rapid scale, there are major challenges associated with digital learning when compared with brick and mortar classrooms. One of many challenges is how to ensure quality learning for students. Digital platforms might overpower physical classrooms in terms of content quality but when it comes to understanding whether students are able to grasp the content in a live class scenario is yet an open-end challenge. In a physical classroom during a lecturing teacher can see the faces and assess the emotion of the class and tune their lecture accordingly, whether he is going fast or slow. He can identify students who need special attention.

Digital classrooms are conducted via video telephony software program (ex-Zoom) where it’s not possible for medium scale class (25-50) to see all students and access the mood. Because of this drawback, students are not focusing on content due to lack of surveillance.

While digital platforms have limitations in terms of physical surveillance but it comes with the power of data and machines which can work for you. It provides data in the form of video, audio, and texts which can be analyzed using deep learning algorithms.

Deep learning backed system not only solves the surveillance issue, but it also removes the human bias from the system, and all information is no longer in the teacher’s brain rather translated in numbers that can be analyzed and tracked.The solution to this problem is by recognizing facial emotions.

I have built a deep learning model which detects the real time emotions of students through a webcam so that teachers can understand if students are able to grasp the topic according to students' expressions or emotions and then deploy the model. The model is trained on the dropbox dataset .This dataset consists of 28000 images, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised. Here is the dataset link:- https://www.dropbox.com/s/si11cws2pyho1bp/archive.zip

###  Introduction

Emotion recognition is the process of identifying human emotion. People vary widely in their accuracy at recognizing the emotions of others. Use of technology to help people with emotion recognition is a relatively nascent research area. Generally, the technology works best if it uses multiple modalities in context. To date, the most work has been conducted on automating the recognition of facial expressions from video, spoken expressions from audio, written expressions from text, and physiology as measured by wearables.

Facial expressions are a form of nonverbal communication. Various studies have been done for the classification of these facial expressions. There is strong evidence for the universal facial expressions of seven emotions which include: neutral happy, sadness, anger, disgust, fear, and surprise. So it is very important to detect these emotions on the face as it has wide applications in the field of Computer Vision and Artificial Intelligence. These fields are researching on the facial emotions to get the sentiments of the humans automatically.

### Model Building

#### Dependencies
•	Python 3

•	Tensorflow 2.0

•	Streamlit

•	Streamlit-Webrtc

•	OpenCV

### Model Creation

Transfer learning (TL) is a research problem in machine learning (ML) that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem. For example, knowledge gained while learning to recognize cars could apply when trying to recognize trucks. This area of research bears some relation to the long history of psychological literature on transfer of learning, although formal ties between the two fields are limited. From the practical standpoint, reusing or transferring information from previously learned tasks for the learning of new tasks has the potential to significantly improve the sample efficiency of a reinforcement learning agent.

## Deployment

In this repository I have made a front end using streamlit .Streamlit doesn’t provide the live capture feature itself, instead uses a third party API. I have used streamlit-webrtc which helped to deal with real-time video streams. Image captured from the webcam is sent to VideoTransformer function to detect the emotion. Then this model was deployed on amazon web services Ec2 Instances     AWS 

```bash
  Link:- http://18.118.198.106:8501/
```

  
## Acknowledgements

 - [Krish naiik]()
 - [Almabetter](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

  
## Appendix

Any additional information goes here

  ```bash
  Link:- http://18.118.198.106:8501/
```

  ❖ https://towardsdatascience.com/face-detection-recognition-and-emotion-detection-in-8-lin es-of-code-b2ce32d4d5de 
  
  ❖ https://towardsdatascience.com/video-facial-expression-detection-with-deep-learning-appl ying-fast-ai-d9dcfd5bcf10 
  
  ❖ https://github.com/atulapra/Emotion-detection 
  
  ❖ https://medium.com/analytics-vidhya/building-a-real-time-emotion-detector-towards-machi ne-with-e-q-c20b17f89220
