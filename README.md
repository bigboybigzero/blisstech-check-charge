# Blisstech Check charge

แอพเช็ครุ่นมือถือว่าชาร์จกับหัว **PD 36W** และ **PD 100W** ของ Blisstech ได้กี่วัตต์ พร้อมปุ่มคัดลอกสคริปต์ส่งลูกค้า

เปิดใช้งาน: https://bigboybigzero.github.io/blisstech-check-charge/

## แก้ข้อมูลรุ่นมือถือ
แก้ที่ไฟล์ `data.js` (1 แถว = 1 รุ่น) แล้ว commit — เว็บจะอัปเดตเองภายใน 1–2 นาที

- `pd36` / `pd100` = วัตต์ที่ได้กับหัว Mini 36W / Pro 100W
  - หัว **Mini 36W** = PD + **UFCS** (ไม่มี PPS) — เครื่องที่รองรับ UFCS จะได้เต็มกำลังหัว (ร้านเทสกับ OPPO Find X9 Ultra ได้ 36W จริง) เครื่องที่ไม่รองรับจะได้แค่เส้น PD ธรรมดา (ราว 10–18W)
  - หัว **Ambient Light 55W** / **Pro 100W** = PD + PPS — ใช้กับ Xiaomi / vivo / Honor ที่ไม่มี UFCS ได้ดีกว่ามาก
- `conf` = `high` มีผลทดสอบ/สเปคทางการ · `medium` อนุมาน · `low` ค่าประมาณ
- `src` = แหล่งข้อมูล
