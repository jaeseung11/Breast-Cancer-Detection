# Breast-Cancer-Detection_project

![image](https://user-images.githubusercontent.com/114135983/229929820-8f6fdc6c-edbc-4f3a-bb9f-c6d8b958ee8e.png)

kaggle: RSNA Screening Mammography Breast Cancer Detection

## 1. 프로젝트 주제
  - 딥러닝(CV)을 활용한 유방암 분류 

## 2. 목표
  - 미국 여성의 유방암 이미지를 보고 EDA를 실시후 적절한 CV 모델링을 찾고 정확성을 높이는 것.
  
## 3. 평가방법
Submissions are evaluated using the probabilistic F1 score (pF1).
![image](https://user-images.githubusercontent.com/114135983/229932707-205075e8-25df-4559-9f03-8a5edc04206c.png)

This extension of the traditional F score accepts probabilities instead of binary classifications. 
You can find a Python implementation here.


## 3. 팀 구성 및 역할
  - 김재승; EDA 및 노션 정리 파트
  - 우현;   CV 모델링
  - 배재한;  CV 모델링 

## 4. 진행 순서
  -EDA 시작 -> 모델링

## 5. 데이터 소개

Note: The dataset for this challenge contains radiographic breast images of female subjects.
The goal of this competition is to identify cases of breast cancer in mammograms from screening exams. It is important to identify cases of cancer for obvious reasons, but false positives also have downsides for patients. As millions of women get mammograms each year, a useful machine learning tool could help a great many people.
This competition uses a hidden test. When your submitted notebook is scored the actual test data (including a full length sample submission) will be made available to your notebook.

Files
[train/test]_images/[patient_id]/[image_id].dcm The mammograms, in dicom format. You can expect roughly 8,000 patients in the hidden test set. There are usually but not always 4 images per patient. Note that many of the images use the jpeg 2000 format which may you may need special libraries to load.
sample_submission.csv A valid sample submission. Only the first few rows are available for download.
[train/test].csv Metadata for each patient and image. Only the first few rows of the test set are available for download.

site_id - ID code for the source hospital.
patient_id - ID code for the patient.
image_id - ID code for the image.
laterality - Whether the image is of the left or right breast.
view - The orientation of the image. The default for a screening exam is to capture two views per breast.
age - The patient's age in years.
implant - Whether or not the patient had breast implants. Site 1 only provides breast implant information at the patient level, not at the breast level.
density - A rating for how dense the breast tissue is, with A being the least dense and D being the most dense. Extremely dense tissue can make diagnosis more difficult. Only provided for train.
machine_id - An ID code for the imaging device.
cancer - Whether or not the breast was positive for malignant cancer. The target value. Only provided for train.
biopsy - Whether or not a follow-up biopsy was performed on the breast. Only provided for train.
invasive - If the breast is positive for cancer, whether or not the cancer proved to be invasive. Only provided for train.
BIRADS - 0 if the breast required follow-up, 1 if the breast was rated as negative for cancer, and 2 if the breast was rated as normal. Only provided for train.
prediction_id - The ID for the matching submission row. Multiple images will share the same prediction ID. Test only.
difficult_negative_case - True if the case was unusually difficult. Only provided for train.


## 6. 


