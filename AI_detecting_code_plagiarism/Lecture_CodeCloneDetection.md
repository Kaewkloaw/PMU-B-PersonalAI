## AI for detecting code plagiarism
***
including 
* What are code clone?
* วิธีสร้าง MML ตรวจจับโค้ดที่เหมือนกัน
* วิธีนำ MML ตรวจจับโค้ดที่เหมือนกัน
* วิธีวัดประสิทธิภาพ MML ที่สร้างขึ้น เชิงความแม่นยำ
* วิธีวัดประสิทธิภาพ MML ที่สร้างขึ้น เชิงเครื่องมือ
* สรุปและแนวทางต่อในอนาคต
1. What are code clone? ความเหมือนกันของ code
![image](https://github.com/user-attachments/assets/50d90739-7ebe-4ea3-93b8-34fb54a20c5e)

ประเภทของ code clone มี 4 ชนิด
![image](https://github.com/user-attachments/assets/05899da0-36dc-45a8-b279-ecefee0eba67)
![image](https://github.com/user-attachments/assets/7a75fe70-c950-4eb5-8763-8ec6b873f457)

การตรวจสอบ code clone detection process
![image](https://github.com/user-attachments/assets/39c5ad09-633e-4433-b719-0da9843baa5a)

***
Merry Engine
![image](https://github.com/user-attachments/assets/fc4b1098-0a4a-448e-9907-825f1d3a6d12)
***

2. วิธีสร้าง MML ตรวจจับโค้ดที่เหมือนกัน
   มี 3 ขั้นตอน ได้แก่
* เก็บและเตรียมข้อมูล
* สร้าง code matrics
* เลือก ML models
  
  2.1 เก็บและเตรียมข้อมูล : ใช้ฐานข้อมูล BigCloneBench
  ![image](https://github.com/user-attachments/assets/66b7ac40-4414-42d9-ba55-9b50e09de729)
  วิธีเอาข้อมูลจาก BigCloneBench
  ![image](https://github.com/user-attachments/assets/c6fe7868-93e1-4c46-adfb-788ce033472a)
  แบ่งข้อมูลเป็น Training set and Testing set
  ![image](https://github.com/user-attachments/assets/24b98ea2-4d46-4add-9849-7af0b007d1ce)
  2.2 code matrics มี 2 แบบ
  ![image](https://github.com/user-attachments/assets/592db53b-b09c-404d-b9a5-fa74b60e2368)
  1) Syntactic metrics
 ![image](https://github.com/user-attachments/assets/4195dad0-65c9-4646-830c-0f73869aeda7)
      Syntactic code metrics
      ![image](https://github.com/user-attachments/assets/823a14f2-1228-420f-9e06-5b93fa6bd7c7)
  2) Semantic metrics
  ![image](https://github.com/user-attachments/assets/0aca3b68-8bb4-4b2e-97b6-f888351a2012)
     code2vec
     ![image](https://github.com/user-attachments/assets/87eb1333-11b5-4550-b676-e5272660442a)
     ***
Syntactic metrics vs Semantic metrics
![image](https://github.com/user-attachments/assets/d7fa2a21-f9d4-48ba-b462-7f591ff4a097)
ML model 
![image](https://github.com/user-attachments/assets/bd033539-280a-4e90-a580-7df54c69d9c9)

3. วิธีนำ MML ตรวจจับโค้ดที่เหมือนกัน
![image](https://github.com/user-attachments/assets/90355645-e7f9-4431-961b-9d38baabf537)
System Architecture
![image](https://github.com/user-attachments/assets/3caa01f5-9d17-4d98-92d9-9ed8f07831b7)
Framework & Tools
![image](https://github.com/user-attachments/assets/34043710-e7b7-4d3b-973a-1468e121b8ba)
Github Integration
![image](https://github.com/user-attachments/assets/17559852-a793-44de-96bc-013fefb274dd)

4. วิธีวัดประสิทธิภาพ MML ที่สร้างขึ้น เชิงความแม่นยำ
Evalution
![image](https://github.com/user-attachments/assets/4ce58aaf-871c-419f-81e8-963fde133a32)
RQ1 :  ประเมินความแม่นยำการตรวจจับโค้ดที่เหมือนกันของ BigCloneBench
![image](https://github.com/user-attachments/assets/972a5d9a-6a8d-4cca-91f4-2a0eb27e1478)
![image](https://github.com/user-attachments/assets/5d00b130-f594-4050-8e8c-ec25ee7c67ce)
![image](https://github.com/user-attachments/assets/b6d1e2d9-95d5-4355-938a-2ca152f1bdf9)
![image](https://github.com/user-attachments/assets/1ccbdc73-5d46-47c6-856b-94d7079d2763)
![image](https://github.com/user-attachments/assets/df36a8ed-df8e-4dc2-b183-df085297868b)

RQ2 : ประเมินความแม่นยำการตรวจจับโค้ดที่เหมือนกันบน software project
![image](https://github.com/user-attachments/assets/4605bc5a-0cb8-4444-8d30-29e92bf12160)
![image](https://github.com/user-attachments/assets/10ffde39-beb3-439a-9a4b-dcfb8a7f3ff3)
case 1 เหมือนกัน100%
![image](https://github.com/user-attachments/assets/bcd57473-f9a6-48b5-9bbb-94b961f2f9ab)
case 2 คล้ายกันมาก ต่างแค่ชื่อตัวแปร
![image](https://github.com/user-attachments/assets/21b985a5-487f-4dcc-93b3-8a264f52385c)
case 3 คล้ายกัน แต่เพิ่มลดบรรทัด
![image](https://github.com/user-attachments/assets/c7e4472e-3044-48f5-9174-5c88cb955e59)
case 4 คล้ายกัน แต่ไม่เหมือนกัน
![image](https://github.com/user-attachments/assets/3401c885-ba51-4c5d-8e5b-76b0eeb33070)

5. วิธีวัดประสิทธิภาพ MML ที่สร้างขึ้น เชิงเครื่องมือ
target 2 กลุ่ม
![image](https://github.com/user-attachments/assets/ff20cc9b-7b62-443e-a7a2-e51d8585a84f)
แบ่งเป็น 2 กลุ่ม คนละเครื่องมือ
![image](https://github.com/user-attachments/assets/61694bd4-0581-4cf2-b90d-ece886815047)
![image](https://github.com/user-attachments/assets/fed25257-f4ec-4e30-9169-aa281664f283)
แบบฟอร์มสำรวจความคิดเห็น
![image](https://github.com/user-attachments/assets/3820b515-7cca-469b-92f5-bd09d0ddc39c)
![image](https://github.com/user-attachments/assets/ff5a53bc-7a77-4ea6-8c53-836f9830f967)
![image](https://github.com/user-attachments/assets/77f0f76a-d6f2-4aa1-a838-621df43b9a1c)
สรุป : เครื่องมือเราตอบโจทย์ผู้ใช้งาน

7.  สรุปและแนวทางต่อในอนาคต

สรุป
![image](https://github.com/user-attachments/assets/16c209b1-e9ea-481d-9a67-50e1521063a4)
ปัญหา & ข้อจำกัด
![image](https://github.com/user-attachments/assets/63b25511-9be2-4ce3-b4ad-24d18a4d790b)
การทำงานในอนาคต
![image](https://github.com/user-attachments/assets/16821044-4fce-4a61-b7c6-5688cbf93bdd)



  



