# เอกสารขอบเขตโครงการ (Scope Document)
## โครงการ: Definition Dash (MVP Phase)

### 1. วัตถุประสงค์ (Objectives)
เพื่อพัฒนา Web Application สำหรับทดสอบคำศัพท์ (Vocabulary Quiz) ในรูปแบบ "Definition Dash" โดยเน้นการใช้งานบนโทรศัพท์มือถือ (Mobile First) เป็นหลัก เพื่อความสะดวกและรวดเร็วในการเรียนรู้ โดยไม่ต้องมีการลงทะเบียนเข้าใช้งาน

### 2. ขอบเขตของระบบ (Scope)

#### ฟังก์ชันที่อยู่ในขอบเขต (IN-SCOPE - Phase 1)
* **Guest Access:** ผู้ใช้งานสามารถเข้าเล่นได้ทันทีโดยไม่ต้องสมัครสมาชิกหรือเข้าสู่ระบบ
* **Quiz Mechanics:**
    * ระบบจับเวลา (Countdown Timer)
    * การสุ่มคำถาม/คำศัพท์
    * การคำนวณคะแนนหลังจบเกม
* **Data Flow:**
    * การส่งข้อมูลคะแนนและสถานะระหว่างหน้าเว็บผ่าน URL Parameters (Query Strings)
* **User Interface:**
    * ออกแบบมาสำหรับหน้าจอ Mobile (Mobile Viewport Only)

#### ฟังก์ชันที่อยู่นอกขอบเขตในเฟสนี้ (OUT-SCOPE / Future Plans)
* **Authentication:** ระบบ Login/Register (วางแผนในอนาคต)
* **Persistent Database:** การบันทึกประวัติคะแนนลงฐานข้อมูลถาวร
* **Desktop Responsive:** การจัดหน้าจอสำหรับ Desktop (ปัจจุบันแสดงผลแบบ Mobile View)
* **Theme Customization:** Dark Mode/Light Mode