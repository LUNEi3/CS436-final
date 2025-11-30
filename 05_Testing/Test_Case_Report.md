# รายงานการทดสอบ (Test Case Report)
รูปภาพการเทสของ User อยู่ที่ Folder `05_Testing\tester`

| TC ID | Test Scenario | Input Data | Expected Output | Actual Result | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TC-01** | เข้าหน้าแรก (Landing Page) | URL: `/` | แสดงปุ่ม Start และ Title บนขนาดจอ Mobile | Pass | ✅ Pass |
| **TC-02** | กรอกชื่อ (ภาษาอังกฤษ) | `Nomnom` | เปลี่ยนหน้าไปยังหน้า Home โดยแสดงชื่อกรอกมาถูกต้อง | Pass | ✅ Pass |
| **TC-03** | กรอกชื่อ (ภาษาไทย) | `สมพง` | เปลี่ยนหน้าไปยังหน้า Home โดยแสดงชื่อภาษาไทยถูกต้อง | ชื่อแสดงผลเป็นต่างดาว หรือ URL Error | ❌ Fail |
| **TC-04** | เริ่มทำแบบทดสอบ | คลิกปุ่ม Start | เปลี่ยนหน้าไปยังหน้า Quiz และเริ่มนับเวลา | Pass | ✅ Pass |
| **TC-05** | การนับถอยหลัง (Timer) | รอเวลาผ่านไป 60 วินาที | ตัวเลขเวลานับถอยหลังลดลงเรื่อยๆ จนถึง 0 | Pass | ✅ Pass |
| **TC-06** | การส่งคะแนนไปหน้าผลลัพธ์ | ตอบถูก 5 ข้อ แล้วจบเกม | URL หน้า Result มี parameter คะแนน (e.g. `?score=5`) และหน้าจอแสดงคะแนน 5 | Pass | ✅ Pass |
| **TC-07** | ปุ่มเล่นอีกครั้ง (Play Again) | คลิกปุ่ม Play Again ที่หน้า Result | กลับไปหน้า Start หรือหน้า Quiz เพื่อเริ่มใหม่ | Pass | ✅ Pass |
| **TC-08** | Mobile Layout Display | เปิดบน Desktop | UI ยังคงจัดกึ่งกลางหรือแสดงผลแบบ Mobile View ไม่แตกเลอะเทอะ | Pass | ✅ Pass |
| **TC-09** | ตรวจสอบชื่อว่าง (Empty Validation) | กด Start โดยไม่กรอกชื่อ | เปลี่ยนหน้าไปยังหน้า Home โดยแสดงชื่อเป็น "Guest" | Pass | ✅ Pass |
| **TC-10** | การตอบถูก (Correct Answer) | เลือกข้อที่ถูก | คะแนนสะสมเพิ่มขึ้น +1 (ตรวจสอบผ่าน Console หรือ UI) | Pass | ✅ Pass |
| **TC-11** | การตอบผิด (Wrong Answer) | เลือกข้อที่ผิด | คะแนนสะสมลดลง -1 (ตรวจสอบผ่าน Console หรือ UI) | Pass | ✅ Pass |
| **TC-12** | จบเกมเมื่อเวลาหมด (Time's up) | ปล่อยเวลาจนเหลือ 0 วินาที | ระบบตัดเข้าหน้า Result อัตโนมัติทันที | Pass | ✅ Pass |
| **TC-13** | ชื่อยาวเกินกำหนด (Overflow UI) | กรอก `AlexanderWolffeschlegelsteinhausenbergerdorff` | ชื่อแสดงผลครบถ้วน หรือตัดคำสวยงามไม่ล้นจอ | ชื่อทะลุกรอบ UI หรือปุ่มตกขอบจอ | ❌ Fail |
| **TC-14** | อักขระพิเศษในชื่อ (URL Safety) | กรอก `M&M` | แสดงชื่อ `M&M` ในหน้าถัดไป | Pass | ✅ Pass |
| **TC-15** | การรีเฟรชหน้าจอขณะเล่น (Refresh) | กด F5 หรือ Refresh ระหว่างทำข้อสอบ | รีเซ็ตเกมใหม่ หรือ กลับไปหน้า Start | Pass | ✅ Pass |
| **TC-16** | การโกงคะแนนผ่าน URL (Security) | แก้ URL เองเป็น `result?score=999` | ระบบตรวจสอบความถูกต้องและไม่แสดงคะแนนปลอม | Pass | ✅ Pass |