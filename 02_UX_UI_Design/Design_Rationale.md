# Design Rationale (เหตุผลในการออกแบบ)

## 1. User Interface (UI) Design
* **Mobile-Only Layout:** เนื่องจากข้อจำกัดด้านเวลาและพฤติกรรมกลุ่มเป้าหมายที่เน้นเล่นเกมสั้นๆ (Micro-learning) จึงออกแบบ UI ให้รองรับขนาดหน้าจอ Mobile เป็นหลัก (Portrait Mode) เพื่อโฟกัสประสบการณ์การใช้งานให้ดีที่สุดในอุปกรณ์เดียว
* **Clean & Minimalist:** เน้นความเรียบง่าย ตัดองค์ประกอบที่ไม่จำเป็นออก เพื่อให้ผู้ใช้โฟกัสที่คำถามและตัวจับเวลา
* **Visual Hierarchy:** ใช้ขนาดตัวอักษรที่ใหญ่และปุ่มที่กดง่าย (Thumb-friendly zone) เหมาะกับการใช้งานบนมือถือ

## 2. User Experience (UX) Flow
* **Frictionless Entry:** ตัดขั้นตอนการ Login ออกเพื่อให้ผู้ใช้เข้าถึง Content ได้เร็วที่สุด (Low Barrier to Entry)
* **Stateless Flow:** ใช้การส่งข้อมูลผ่าน URL Query ทำให้แอปพลิเคชันมีความเบา ไม่ต้องรอโหลดข้อมูลจาก Server และลดความซับซ้อนในการจัดการ State