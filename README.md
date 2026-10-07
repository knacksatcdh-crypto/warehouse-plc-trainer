# Warehouse PLC Trainer — ขึ้นเว็บด้วย Render.com

ไฟล์ในโฟลเดอร์นี้
- `index.html` — ตัวโปรแกรมทั้งหมด (ไฟล์เดียว ไม่ต้อง build)
- `render.yaml` — ตั้งค่าให้ Render สร้าง Static Site อัตโนมัติ

## ขั้นตอน (ฟรี ~5 นาที)
1. สมัคร/เข้า https://github.com → กด **New repository** ตั้งชื่อ เช่น `warehouse-plc-trainer` (Public หรือ Private ก็ได้) → Create
2. ในหน้า repo กด **uploading an existing file** → ลาก `index.html` และ `render.yaml` เข้าไป → **Commit changes**
3. เข้า https://dashboard.render.com (ล็อกอินด้วย GitHub ได้) → **New +** → **Blueprint**
4. เลือก repo `warehouse-plc-trainer` → Render จะอ่าน `render.yaml` เอง → กด **Apply / Deploy Blueprint**
5. รอ 1–2 นาที จะได้ลิงก์ประมาณ `https://warehouse-plc-trainer.onrender.com` เปิดได้ทุกเครื่อง

> ไม่อยากใช้ Blueprint: **New +** → **Static Site** → เลือก repo → Build Command เว้นว่าง (หรือ `echo ok`) → Publish Directory ใส่ `.` → Create Static Site

## อัปเดตเวอร์ชันใหม่
อัปโหลด `index.html` ตัวใหม่ทับใน GitHub (Add file → Upload files) → Render จะ Deploy ใหม่ให้อัตโนมัติ

## หมายเหตุ
- งานที่เขียน (Ladder, HMI, Watch) เก็บในเบราว์เซอร์ของแต่ละเครื่อง — ใช้ปุ่ม 💾 บันทึก เพื่อดาวน์โหลดไฟล์ .json เก็บไว้ (บนเว็บ Render ปุ่มบันทึก/ดาวน์โหลดใช้ได้ปกติ)
- Static Site ของ Render ฟรีและไม่หลับ (ต่างจาก Web Service)
