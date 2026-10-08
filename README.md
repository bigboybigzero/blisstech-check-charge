# Blisstech Check charge

แอพเช็ครุ่นมือถือว่าชาร์จกับหัว **PD 36W** และ **PD 100W** ของ Blisstech ได้กี่วัตต์ พร้อมปุ่มคัดลอกสคริปต์ส่งลูกค้า

เปิดใช้งาน: https://bigboybigzero.github.io/blisstech-check-charge/

## แก้ข้อมูลรุ่นมือถือ
แก้ที่ไฟล์ `data.js` (1 แถว = 1 รุ่น) แล้ว commit — เว็บจะอัปเดตเองภายใน 1–2 นาที

- `pd36` / `pd100` = วัตต์ที่ได้กับหัว Mini 36W / Pro 100W
  - หัว **Mini 36W** = PD + **PPS** (+ UFCS) — ร้านเทสแล้วได้ 36W เต็มหัวทั้ง OPPO Find X9 Ultra และ Xiaomi 17 Ultra เครื่องที่รองรับ PPS/UFCS จึงได้ min(36W, เพดานของเครื่อง) ส่วน Huawei/Honor ที่ไม่มีทั้ง PPS และ UFCS ยังได้แค่เส้น PD (ราว 10–12W)
  - หัว **Ambient Light 55W** / **Pro 100W** = PD + PPS — ต่างจาก Mini ที่กำลังไฟ ใช้กับเครื่องที่รับได้เกิน 36W จะเห็นผลชัด
- `conf` = `high` มีผลทดสอบ/สเปคทางการ · `medium` อนุมาน · `low` ค่าประมาณ
- `src` = แหล่งข้อมูล
