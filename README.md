# Definition Dash

Definition Dash คือเว็บแอปพลิเคชัน Vocabulary Quiz ที่พัฒนาขึ้นเป็น Final Project รายวิชา Software Engineering (CS436) เน้นความรวดเร็วในการเรียนรู้ผ่านหน้าจอมือถือ โดย <u> **ปริวัฒน์ นิรานนท์ 1670702230 CS436 section: 227C** </u>

## Notes
**ไฟล์ใน Folder [`/04_Implementation/definition-dash`](04_Implementation/definition-dash) เป็น version เก่า แนะนำให้ไปดูตามลิงค์ด้านล่างนี้**

GitHub: https://github.com/LUNEi3/definition-dash<br />
Deployment Link: https://definition-dash-liart.vercel.app/
Video Manual: [`06_Deployment_Review/userManual.mov`](06_Deployment_Review/userManual.mov)

## Current Status (MVP)
โปรเจกต์นี้อยู่ในระยะ MVP (Minimum Viable Product) โดยเน้นฟังก์ชันหลักคือการทำแบบทดสอบและการแสดงผลคะแนน
* **Platform:** Mobile Web Application (Optimized for Mobile Views)
* **Data:** Stateless (No Database), Data passed via URL

## Features
* **Quick Start:** เข้าเล่นได้ทันทีไม่มี Login
* **Timer Challenge:** ระบบจับเวลาเพิ่มความท้าทาย
* **Instant Feedback:** สรุปคะแนนทันทีหลังจบเกม

## Tech Stack
* **Frontend:** Next.js, React, Tailwind CSS
* **Language:** TypeScript

## Installation & Run

1.  **Clone Repository**
    ```bash
    git clone [https://github.com/LUNEi3/definition-dash.git](https://github.com/LUNEi3/definition-dash.git)
    cd definition-dash
    ```

2.  **Install Dependencies**
    ```bash
    npm install
    ```

3.  **Run Development Server**
    ```bash
    npm run dev
    ```
    เปิด Browser ไปที่ `http://localhost:3000` (แนะนำให้เปิดโหมด Inspect -> Mobile View)
