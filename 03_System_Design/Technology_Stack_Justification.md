# Technology Stack Justification

## 1. Frontend: Next.js & React
* **เหตุผล:** เลือกใช้ Next.js เพื่อโครงสร้างโปรเจกต์ที่เป็นระเบียบและการจัดการ Routing ที่มีประสิทธิภาพ แม้ปัจจุบันจะยังไม่ได้ใช้ฟีเจอร์ Server-Side ขั้นสูง แต่เตรียมพร้อมสำหรับการขยายระบบในอนาคต

## 2. Styling: Tailwind CSS
* **เหตุผล:** ช่วยให้จัด Layout แบบ Mobile ได้รวดเร็วมาก ผ่าน Utility Classes และสามารถปรับแต่ง Design System ได้ง่ายโดยไม่ต้องเขียน CSS เองทั้งหมด

## 3. Data Handling: URL Parameters (Query Strings)
* **เหตุผล:** สำหรับ MVP ที่ไม่มี Database การส่งข้อมูล (เช่น คะแนน, จำนวนข้อที่ถูก) ผ่าน URL เป็นวิธีที่ง่ายและรวดเร็วที่สุดในการส่งค่าจากหน้า Quiz ไปยังหน้า Result โดยไม่ต้องใช้ Global State Management (เช่น Redux) หรือ Backend

## 4. Language: TypeScript
* **เหตุผล:** ช่วยดักจับ Error ระหว่างการเขียน Code โดยเฉพาะการจัดการ Data Type ที่รับส่งผ่าน Props และ URL ทำให้ลดบั๊กที่อาจเกิดขึ้นตอน Runtime