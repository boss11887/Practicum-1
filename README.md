# ชื่อโครงงาน : ที่ใส่รหัสผ่านเพื่อปลดล็อกประตูนิรภัย
โครงงานนี้เป็นส่วนหนึ่งของรายวิชา 01204223 Practicum for Computer Engineering ภาคปลาย ปีการศึกษา 2564 หมู่ 11,12

### สมาชิกผู้จัดทำ:  
> :shipit:นิสิตภาควิชาวิศวกรรมคอมพิวเตอร์ คณะวิศวกรรมศาสตร์ มหาวิทยาลัยเกษตรศาสตร์ วิทยาเขตบางเขน:shipit:  

6310500325 ปองภพ ไกรรวีโรจ<br>
6310500066 สุคชาธัม เซียวศิริถาวร<br>
6310500350 วิชญ์นพัฒน์ จำปาเรือง<br>
6310500287 ตะวันฉาย ฉัตรกุล ณ อยุธยา<br>


## รายละเอียดไฟล์ Source Code :  
### Hardware   
```
main
│   practicum.py : การส่งค่าระหว่าง backend กับ hardware
│
└───face_recognition
│   │   blink.ino : โปรกรมสำหรับการควบคุม Hardware ทุกอย่าง
│
```
### Frontend  
```
main
│   1_upload_picture.py : โปรแกรมสำหรับการอัพโหลดรูปภาพผู้ใช้งาน   
│   0_frontend.py : GUI สำหรับการแสดงผล การสแกนหน้าเพื่อเข้าใช้งาน สถานะเปิดปิดของประตู
│
```
### Backend  
    
```
main
│   Can_Pass : หน้าของคนทั้งหมดที่สามารถสแกนหน้าเพื่อผ่านเข้าประตูได้
│   Can_not_Pass : หน้าของคนทั้งหมดที่ไม่สามารถสแกนหน้าเพื่อผ่านเข้าประตู
│   Picture for test : ใบหน้าของผู้คนทั้งหมดสำหรับการดสอบ
│
└───log
│   │   1_status.log : ก็บประวัติการใช้งาน (เก็บทั้งหมดไม่ว่าจะผ่านหรือไม่ผ่าน)  
│   │   1_status.txt : status ปัจจุบันของประตุเปิดหรือปิด
│   
│   0_backend.py : โปรแกรมสำหรับการ detect ใบหน้า, ควบคุมการแสดงผล, ควบคุมการเปิดปิดประตู
```
## รายการไลบรารี/เฟรมเวิร์คที่ใช้ :
### Hardware - 
usbdrv.h, Wire.h, Servo.h, LiquidCrystal_I2C.h  

### Frontend - 
logging, tkinter, datetime, turtle, cv2, PIL  

### Backend - 
face_recognition, cv2, numpy, time, os, datetime  

## รายการอุปกรณ์ฮาร์ดแวร์ที่ใช้ :
<ul>
  <li>Board NodeMCU - ATmega328p (Practicum Board v3.2 CPE. KU 2020-11) 2 ตัว</li>
  <li>Peripheral board (PRACTICUM PROTOBOARD CPE. KU) 3 ชิ้น</li>
  <li>สายแพ 3 เส้น</li>
  <li>Switch button กดติดปล่อยดับแบบ 4 ขา ขนาด 6x6x5 mm 6 ชิ้น</li>
  <li>Servo SG90S 1 ตัว</li>
  <li>1602 LCD (Blue Screen) 16x2 LCD with backlight of the LCD screen พร้อม I2CInterface 5V 1 ชุด</li>
  <li>Jumper wire Female-Female 4 เส้น</li>
  <li>Jumper wire Male-Female 3 เส้น</li>
  <li>Pin header ที่เพิ่มเข้ามา มีหลากหลายขนาด ดังนี้</li>
    <ul>
      <li>ขนาด 5x2 : 3 ชิ้น</li>
      <li>ขนาด 2x1 : 1 ชิ้น</li>
      <li>ขนาด 1x1 : 5 ชิ้น</li>
    </ul>
  </ul>
