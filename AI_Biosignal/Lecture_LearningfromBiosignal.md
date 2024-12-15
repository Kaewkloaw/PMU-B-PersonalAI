## Sleep stage scoring from biosignal 
***
Biosignals: ข้อมูลทางการแพทย์
* คลื่นไฟฟ้าสมอง
* คลื่นไฟฟ้าหัวใจ

Sleeping problem
![image](https://github.com/user-attachments/assets/1d50fadf-32f3-46f1-b378-46f26a6cb7ca)
* นอนหลับไม่สนิท
* อุปกรณ์ไม่เพียงพอ / ยากต่อการใช้งาน
* Sleep Apnea: โรคหยุดหายใจขณะหลับ

Challenges in Treatment
* ในโรงพยาบาลมีผู้เชี่ยวชาญหรือเตียงไม่เพียงพอต่อจำนวนผู้ป่วย
* ดูอาการ 1 คืนไม่สามารถเก็บข้อมูลได้ครบถ้วน

***

1. การวิเคราะห์คลื่นสัญญาณจากร่างกายคน (Biosignal Analysis)
   ![image](https://github.com/user-attachments/assets/2edd49a8-0388-4270-b400-3a1756fc21d2)
   พยายามใช้ Deep Learning เพื่อกำจัดข้อ 1 และ 2
   ![image](https://github.com/user-attachments/assets/e096d692-9145-495e-a4dd-0a66d8fec5fa)
2. การวิเคราะห์การนอน (Sleep Stage Scoring)
   * เก็บข้อมูล
     ![image](https://github.com/user-attachments/assets/8c9b6e2a-c5dc-4e5b-97d9-c1afeea7feae)
   * รายละเอียดข้อมูล
     ![image](https://github.com/user-attachments/assets/1e8fe657-b38b-456c-b142-b8c759ab1c8d)
    ตัวอย่างคลื่นสมอง
    ![image](https://github.com/user-attachments/assets/3114f7c9-c63a-422c-bb97-de5b3c957afa)
    ![image](https://github.com/user-attachments/assets/885bfbdd-11f5-4293-b6b0-b18c72e968cc)
   * การคำนวณ
    ![image](https://github.com/user-attachments/assets/ea648c09-64dc-4128-8e92-9b205d93dd58)
   * ฐานข้อมูล
    ![image](https://github.com/user-attachments/assets/cf14f968-e0d2-40d3-8e6f-c086a78b020f)
3. แบบจำลองสำหรับวิเคราะห์การนอน (Model)
   * DeepSleepNet
     ![image](https://github.com/user-attachments/assets/1fd081fc-7e3a-4a52-8a86-d2091bac3d95)
     ![image](https://github.com/user-attachments/assets/c93bd215-1426-42d1-a00b-f92f4a4f838c)
     แบ่งเป็น CNN-small กับ CNN-Large เพื่อสกัดจุดเด่น
     ![image](https://github.com/user-attachments/assets/a2638c82-e02b-4fe7-9edf-be69a9dad301)
     แต่ละนิวรอนเป็น 1 feature
     ![image](https://github.com/user-attachments/assets/73901a9e-b4f2-43e4-92f3-239c5a0a16b7)
     ใช้ RNN
     ![image](https://github.com/user-attachments/assets/a363e659-c030-4080-8afa-bbbeb7fb895e)
     ![image](https://github.com/user-attachments/assets/b7a40417-d7b0-45ea-980a-49149818b367)
     ![image](https://github.com/user-attachments/assets/4fc6c316-c694-45b2-af76-fa3899c5b4c0)
  * TinySleepNet: พัฒนาจาก DeepSleepNet โดยลดขนาดแต่คงประสิทธิภาพ
    ![image](https://github.com/user-attachments/assets/613d6cb4-3075-42b5-aafa-136b0724763e)
    ![image](https://github.com/user-attachments/assets/ff48c7a2-f3a4-4020-93a4-99c797428ed2)
    ![image](https://github.com/user-attachments/assets/6b6167fa-3a3f-4229-b4a6-e89379d2885b)
    การเทรน
    ![image](https://github.com/user-attachments/assets/bd18d0eb-f4c6-4eaf-8d5c-9c63adbae5af)
    * signal augmentation เพิ่มความหลากหลายของข้อมูล
      ![image](https://github.com/user-attachments/assets/f173c930-af70-46d6-8681-8253d5827e37)
      ![image](https://github.com/user-attachments/assets/23453e81-5298-408e-a4ad-d1990444b836)
4. การวัดผลการวิเคราะห์การนอน (Evaluation)
![image](https://github.com/user-attachments/assets/c3131f12-93a4-40bd-9eb1-3f7acb2e85c2)
* k-fold cross-validation
![image](https://github.com/user-attachments/assets/ad69d9fc-3387-4a8e-8612-cc4e857fbc2d)
ภาพแสดงถึง 5-fold cross-validation
* Confusion Matrix
![image](https://github.com/user-attachments/assets/eb4480b1-18bb-4f7f-a5a4-f98d4dc6968a)
![image](https://github.com/user-attachments/assets/ec4c1859-4bca-42e0-a821-2f197fb49bcf)
การวัด performance
![image](https://github.com/user-attachments/assets/4e614a49-4212-4e23-bc5e-e3446694caf7)
* Hypnogram
![image](https://github.com/user-attachments/assets/a4bb3de5-a298-4b89-b5a0-04b20ef61f4f)
![image](https://github.com/user-attachments/assets/5bd06785-61c8-48ee-9495-5e064e27d99e)



