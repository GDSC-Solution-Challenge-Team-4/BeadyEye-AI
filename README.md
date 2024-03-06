# GDSC Solution Challenge - BeadyEyes
## AI repo

### How to run my code on local environment by using python
---

## Text Recognition based on Hand Landmark (OCR)
### What is it? 
- Read the text indicated by your finger
- You can OCR recognize and retrieve the letter closest to the top of the part you are pointing with your finger.


### Reference
- <a href='https://cloud.google.com/vision/docs/ocr?hl=ko#vision_text_detection_gcs-python'>google-cloud-vision-OCR</a>
- <a href='https://developers.google.com/mediapipe/solutions/vision/hand_landmarker/python'>MediaPipe-Hand landmarks detection</a>


### Enviroment
- python version : 3.11


### How to do?

```
$ git clone https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEye-AI.git && cd BeadyEye-AI/OCR
```
```
$ pip install -r requirements.txt
```

* You need to have a Google Cloud Platform (GCP) key prepared.
* (Google Cloud Platform (GCP) key 가 준비되어 있어야 합니다.)
- <a href = 'https://cloud.google.com/iam/docs/keys-create-delete?hl=ko'>Create GCP key</a>



- After downloading the gcp key, change the file name to “ourAccountKey.json” and place it in the OCR folder.
- (gcp key를 다운받은 후 파일이름을 "ourAccountKey.json"으로 변경한 후 OCR 폴더에 넣어주세요)
  <img src='https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEyes-AI/assets/79080825/f22e64a5-160e-4951-8016-a78020f98c07' width='300'>



You can get the results returned through the following code.
```
$ python -c "from handLandmark import text_pointer_uri; result = text_pointer_uri('{your_image_uri}');print('\nresult: ', result)"
```

You can OCR recognize and retrieve the letter closest to the top of the part you are pointing with your finger.

---
### Example 
#### **Example1**

<img src='https://raw.githubusercontent.com/garden-jun/BeadyEyes-AI/main/OCR/images/testimage.jpg' width='300'></src>
- excute code
![image](https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEyes-AI/assets/79080825/cdc02079-de38-40a3-8c88-dd0f93d96846)
- result

  ![image](https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEyes-AI/assets/79080825/c6ecccca-ab48-40b1-b1e9-d410ed880b9b)


#### **Example2**

<img src='https://raw.githubusercontent.com/garden-jun/BeadyEyes-AI/main/OCR/images/testimage2.jpg' width='500'></src>
- excute code
![image](https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEyes-AI/assets/79080825/ec2b214e-b65b-4d64-9ede-1da7ea78b88e)

- result
  
  ![image](https://github.com/GDSC-Solution-Challenge-Team-4/BeadyEyes-AI/assets/79080825/ac239095-15db-4c1a-bb26-093c2543bbe0)



