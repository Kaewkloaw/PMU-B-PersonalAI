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
  2) Semantic metrics

  



