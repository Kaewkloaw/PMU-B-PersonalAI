## Real-Time Object Detection
***
ตรวจจับวัตถุ โดยต้องคำนึงถึงความแม่นยำในการระบุตำแหน่ง เวลาที่ใช้ในการประมวลผล และการแยกประเภทที่ถูกต้อง
![image](https://github.com/user-attachments/assets/b0d59108-17e0-4270-bdde-6a64b56a7639)

1. ความสำคัญของ Object Detection
![image](https://github.com/user-attachments/assets/4da80f05-e0e1-47fe-a162-d7e8e9f60f70)
Timeline YOLO version
![image](https://github.com/user-attachments/assets/c48ffdf9-6c3f-49b1-96f7-180f6e24977e)
concept YOLO : แบ่งรูปเป็นกริซ S x S grid มีแกน x,y ค่า 0 ถึง 1 ดังนั้นช่องตรงกลาง (0.5,0.5) / w,h คือ ขนาด bounding block / confidence คือ ค่าความน่าจะเป็นของความถูกต้อง
![image](https://github.com/user-attachments/assets/be1dd787-d027-4064-957d-684ad8d58fdb)

2. YOLO Training
![image](https://github.com/user-attachments/assets/11a74d45-cafe-4d57-b680-89494ae02198)
X : input of algorithm
Y : output of algorithm = tensor
B : amount of bounding block
S : amount of grid cell
C : amount of class (can detect)

4. YOLO Architecture
![image](https://github.com/user-attachments/assets/ec5e62b7-770e-4520-9af7-af62fed8fb9a)
แต่ละ layer ทำหน้าไม่เหมือนกัน (CNN)
* Non-maximal suppression : กรองช่องที่ไม่มีรูปภาพ เพิ่มความเร็วในการทำงาน
![image](https://github.com/user-attachments/assets/eaab7c8b-31b6-42cd-8af3-b499479af898)

5. YOLO Prediction
![image](https://github.com/user-attachments/assets/af28053a-af96-4be2-96fc-b61da59198cb)

6. YOLO Objective Function : ลดerror
* Localization loss : Position & Size
![image](https://github.com/user-attachments/assets/4df1b36f-32e5-471d-97a8-394359ed4513)
* Confidence loss
![image](https://github.com/user-attachments/assets/2f6fafbf-71f6-4278-b028-58d36ca17377)

* Classification loss
![image](https://github.com/user-attachments/assets/7b11d351-4eaf-42d2-91e5-2a04f9e10c24)
***
YOLO V8 : ลดความซ้ำซ้อน เพิ่มความแม่นยำ
![image](https://github.com/user-attachments/assets/47bc3cc4-e0bb-4a89-a4e5-fa6c562b732c)
![image](https://github.com/user-attachments/assets/acb85e39-faca-4ab6-b32a-4bfa54071584)
![image](https://github.com/user-attachments/assets/6d8e534f-e488-460b-9603-e73cf3d2cf0e)
