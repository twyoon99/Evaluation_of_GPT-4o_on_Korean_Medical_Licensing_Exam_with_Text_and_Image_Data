<img width="1211" alt="image" src="https://github.com/user-attachments/assets/5ae6de59-bd56-46d8-a932-1e050d30f85a" /># Korea Clinical Datathon 2024 


## Evaluating the performance of GPT-4o on Korean Medical Licensing Examinations using both text and image data (+ possible bias perpetuated in GPT-4o)


### Team Name : Bias, By us!

---


## Introduction
### Background


  - GPT-4o : Multimodal model has been introduced

    
  - There are no studies evaluating the performance of LLM on KMLE yet.

    
  - There are no studies evaluating the Medical Licensing Examination using GPT-4o yet.

    
  - Bias might be perpetuated in LLMs


### Objectives
  - Evaluate GPT-4o’s accuracy on the KMLE using both text and image data

  - Compare the accuracy between providing images and providing text only.

  - Evaluate possible bias perpetuated in GPT-4o

  - Evaluate the impact of different sex and race/ethnicity instructions on the performance of GPT-4o in generating responses to test questions

  - Evaluate accuracy across subjects

  - Evaluate different prompting strategies (ex. CoT vs no CoT)   (CoT: chain of thought prompting)

---

## Methods
### Dataset


  - 2019 ~ 2023 KMLE data
  - With images


### Example
## Provide both text and image context to GPT-4o

  - Question
  5세 남아가 ２시간 전부터 발생한 피부 발진으로 병원에 왔다. 3시간 전에 가족들과 외식을 했고, 식사하고 １시간 후에 몸이 가려워지면서 발진이 나타났다. 체온 36.5℃이다. 피부 사진 (사진 35)이다. 혈액검사 결과는 다음과 같다. 원인 매개체는?
  
  혈색소 13.8 g/dL, 백혈구 9,800/mm3 (중성구 40%, 림프구 52%, 호산구 2%)

![image](https://github.com/user-attachments/assets/79365c78-e945-419d-ad82-10bc6b9f6b2f)

  - Choices
  1. 보체
  2. 히스타민
  3. 브라디키닌
  4. 인터페론감마
  5. 인터루킨-10

---
### Workflow

<img width="1211" alt="image" src="https://github.com/user-attachments/assets/79c0513b-a527-4ef3-ae56-6e86e382ba23" />

<img width="995" alt="image" src="https://github.com/user-attachments/assets/c50df24a-6c6b-4e53-8188-7fee01b555e0" />



