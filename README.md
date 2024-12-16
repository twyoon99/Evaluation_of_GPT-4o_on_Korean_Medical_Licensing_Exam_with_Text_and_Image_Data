# Korea Clinical Datathon 2024 


---
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

  - #### Question
  5세 남아가 ２시간 전부터 발생한 피부 발진으로 병원에 왔다. 3시간 전에 가족들과 외식을 했고, 식사하고 １시간 후에 몸이 가려워지면서 발진이 나타났다. 체온 36.5℃이다. 피부 사진 (사진 35)이다. 혈액검사 결과는 다음과 같다. 원인 매개체는?
  
  혈색소 13.8 g/dL, 백혈구 9,800/mm3 (중성구 40%, 림프구 52%, 호산구 2%)

![image](https://github.com/user-attachments/assets/79365c78-e945-419d-ad82-10bc6b9f6b2f)


  - #### Choices
  1. 보체
  2. 히스타민
  3. 브라디키닌
  4. 인터페론감마
  5. 인터루킨-10

#### Provide both text and image context to GPT-4o


### Workflow

<img width="1213" alt="image" src="https://github.com/user-attachments/assets/98dcc8ed-fa42-465b-95a2-6abd9fb8d02b" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/4f239926-dfa7-40f1-868d-5335d5c41ec1" />


### Full prompt and response example

<img width="1213" alt="image" src="https://github.com/user-attachments/assets/1e640586-2730-476b-b4e6-f1d459ed6c2c" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/83447f3b-989d-4f7d-b590-4246003de00b" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/92b209cc-e00e-4219-b8d6-45c49b9fb76f" />

---
## Results


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/c7953fc2-13b0-4d4b-942b-72fd85256f24" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/a32b4744-287e-4064-b7d5-157dadb78aba" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/3fb3879a-0839-4bff-b054-0b370687e4c9" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/f468536a-dff8-4b05-a2d5-c637a9f60246" />


<img width="1213" alt="image" src="https://github.com/user-attachments/assets/9fc0b6b4-0749-480f-933f-70746e8b9e0f" />


- ### Example of an incorrect GPT-4o response in the “health policy” subject
  - #### Example of an incorrect GPT-4o response that might have been caused by different laws across countries.


__Question__: 콜레라에 걸리면 의사는 어디에 신고해야하는가? (Where should a doctor report if someone contracts cholera?)
__Correct answer in KMLE__ (Korean law): 소속 의료기관의 장 (Head of the affiliated medical institution)


__GPT-4o response__: 관할 보건소장 (Head of the local health center)


__US Law__: Local health jurisdiction


- ### Example of an incorrect GPT-4o response in the “preventive medicine” subject


![image](https://github.com/user-attachments/assets/95ef82d8-9ff9-4acc-908d-d32a81230093)

---
## Discussion


- GPT-4o achieved an accuracy of 0.838 on the KMLE using both text and image data

  
- Questions were provided in Korean.

  
- Providing images compared to providing text only improved accuracy, with marginal statistical significance

  
- Even when the test-taker's sex and race/ethnicity were set differently as instructions to GPT-4o, no bias was observed.

  
- Accuracy was low in the following subjects

  
  - “Health policy”: Different laws across countries?
  - “Preventive medicine”: difficult task for GPT-4o
 
    
- Well-known prompting stratigies such as CoT was indeed necessary.


- ### Future plans
  - #### Manuscript?
 
    - Few shot prompting
   
      
    - Comparison with other local-version models (ex. Bllossom/llama-3-Korean-Bllossom-70B)
   
      
    - Rotation, blurring, etc of images?
   
      
    - Better prompting strategy to guide GPT-4o to refer to images more effectively?
   
      
    - Other MLEs. (ex. USMLE)
   
      
    - More years (ex. 2020~2023)

---
