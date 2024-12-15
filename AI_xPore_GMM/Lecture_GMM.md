## xPore: An AI-Powered App for Bioinformaticians 
***
1. Problem Statement
  * Central Dogma
  ![image](https://github.com/user-attachments/assets/a975de87-7e0f-4edc-ab77-c08d84838f9a)
  * Past vs Current Solution
![image](https://github.com/user-attachments/assets/53b5ea14-5899-48a8-b8be-32cfba44bd43)
  * RNA Sequencing Process
![image](https://github.com/user-attachments/assets/35414b95-51af-4556-9859-8f1d4ed805cc)
  * RNA modifications
![image](https://github.com/user-attachments/assets/1cfa42d7-397e-4627-bd94-40dd097b0c72)
  * Datasets and Requirements Output Table
![image](https://github.com/user-attachments/assets/7340af7d-0f36-4d5e-98c1-8cbc5143e868)
  * Research Objectives
![image](https://github.com/user-attachments/assets/1d450855-7964-4e41-8a21-7b93021d0280)

2. Data Collection and Preparation
จากเครื่องจะได้ไฟล์เป็น Fast5 (สัญญาณไฟฟ้า)
![image](https://github.com/user-attachments/assets/de5c3356-8c62-40f0-a3b3-85b4ad3128e1)
แล้วแปลงจากสัญญาณไฟฟ้ามาเป็น
  * FastQ
  ![image](https://github.com/user-attachments/assets/6bc1cd88-8e1e-4d47-959d-d2e2757f8381)
  * FastA
  ![image](https://github.com/user-attachments/assets/c409cd55-c3e3-4122-a140-fee399560b60)
  * BAM/SAM
  ![image](https://github.com/user-attachments/assets/66628d8a-f232-426d-bda1-d1f4a77bb687)
  * UCSC Genome Browser
  ![image](https://github.com/user-attachments/assets/3897b1be-c154-45cf-a2fb-b748f16141b6)

การทำ Preprocessing จาก Nanopre เพื่อหา Signal-level data analysis
![image](https://github.com/user-attachments/assets/27cee878-4f98-45b1-94f8-6d630fa14aa2)

3. Bayesian (Multi-Sample) - Gaussian Mixture Modeling

![image](https://github.com/user-attachments/assets/454853a1-e90e-40bf-886d-cdc1b1b6ebf6)
  * Guassian 
  แกน y คือ Probability 
  แกน x เป็นสัญญาณไฟฟ้า 
  ![image](https://github.com/user-attachments/assets/532f6e81-d9c7-45a9-a7bc-4d0a11b2eaf4)
* Gaussian Mixture Model (GMM)
  ![image](https://github.com/user-attachments/assets/340dc3e0-01db-4273-bd8f-e34dbc7e090c)\
* GMM Inference
  ![image](https://github.com/user-attachments/assets/b1176516-09c5-4ed4-aa99-c84501694442)
* ภาพรวมของ GMM
  ![image](https://github.com/user-attachments/assets/0c7a26b8-c30f-47a8-9232-397708120978)
Image Classification -> Discriminative มันไม่สามารถสร้างข้อมูลขึ้นมาได้
* Bayesian
![image](https://github.com/user-attachments/assets/8dc677f6-8cab-4cb6-b755-5c16ee06e1a7)
***
Frequentist vs Bayesian
![image](https://github.com/user-attachments/assets/313b8862-9924-4e50-a7d7-9d72ac61e96d)
***
* Multi-Sample
  ![image](https://github.com/user-attachments/assets/dcdcbd60-dd11-41ea-b473-594ae82aa937)
* Speed-Up ML Experiments
  ![image](https://github.com/user-attachments/assets/e354018a-fc83-4b01-b5b1-045dfcdb2fb1)

4. Evaluation 

* Experiment Setup
  ![image](https://github.com/user-attachments/assets/2da586b3-e51b-4537-8bac-bdf6b64a5451)
 Domain Specific Evaluation
 ![image](https://github.com/user-attachments/assets/4a314aed-bd84-4f02-8c16-d38e1c47c760)

* Validation 
![image](https://github.com/user-attachments/assets/6faa4194-62d7-4767-b2c7-979d4e335490)
![image](https://github.com/user-attachments/assets/ff960802-243a-47f2-b398-094f36209c2d)
![image](https://github.com/user-attachments/assets/e7fc7dcc-d355-446f-a878-2bcc0fd501d6)

5. Visualization and Presentation (Deploy / Present Paper)

![image](https://github.com/user-attachments/assets/9288dcd3-8820-4220-8e0b-07c6040213dc)
![image](https://github.com/user-attachments/assets/acca3aca-ea0f-4261-95e9-ea797802b3e9)

6. Future Work

![image](https://github.com/user-attachments/assets/70faed44-faa8-4fff-a8b3-f349e40a0129)
* Domain-Oriented
* Method-Oriented
