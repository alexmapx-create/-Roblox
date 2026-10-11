# DRAGON KINGDOM TYCOON — Storybook build

รุ่นปรับภาพและ UI: แถบไม้ ช่องทรัพยากรสีครีม เหรียญเลเวล/XP ปุ่มหินกลม และหน้าต่างกระดาษ พร้อมเมนู “อาณาจักร” พับได้ เกาะมีหน้าผาน้ำตาล ขอบหญ้า ต้นไม้มีราก อาคารไม้และถิ่นอาศัยสีตามธาตุ มังกรมีดวงตา แก้มและปีกละเอียดขึ้น กล้องปรับระยะตามขนาดจอ

## ดาวน์โหลด

- [ไฟล์ Roblox Studio รุ่นใหม่](downloads/DragonKingdomTycoon-Storybook.rbxl)
- [ZIP source, assets, place, คู่มือและผลตรวจ](downloads/DragonKingdomTycoon-Storybook.zip)
- [SHA256 ของไฟล์ดาวน์โหลด](downloads/SHA256SUMS.txt)

หน้าไฟล์บน GitHub ใช้ปุ่ม **Download raw file** หากเบราว์เซอร์เปิดตัวอย่างแทนการดาวน์โหลด

## เปิดทดสอบ

1. หยุด Play และเปิดไฟล์ `DragonKingdomTycoon-Storybook.rbxl` ด้วย **File → Open from File**
2. กด Play; เริ่มด้วยมังกรสามตัวและถิ่นอาศัยสามแห่ง
3. ปุ่ม **อาณาจักร** เปิดคลัง โรงฟัก ผสมพันธุ์ ประลอง รางวัลและระบบอื่น ๆ ส่วนภารกิจ/สร้าง/ตลาด/ตั้งค่าเข้าถึงจากปุ่มริมจอ
4. รุ่นนี้ใช้ข้อมูลชั่วคราวเฉพาะใน Studio จึงทดสอบ place ที่ยังไม่ Publish ได้ ข้อมูลหายเมื่อหยุด Play; เซิร์ฟเวอร์ที่เผยแพร่ใช้ DataStore เสมอ วิธีทดสอบ save จริงอยู่ใน `docs/STUDIO_SETUP.md` ภายใน ZIP

การตรวจคลาวด์ผ่าน 85 ข้อ (กฎเกม/ความปลอดภัย/การบันทึกจำลอง 61, การเชื่อมต่อ 14, กล้อง 10) พร้อม compile ทุก source, UI/world mocks, assets และ Rojo build ตรวจ source ที่ฝังใน place ครบ

ภาพ `build/preview/DragonKingdomTycoon-Storybook.png` ใน ZIP เป็น offline render จาก geometry/UI source จริง พร้อม metadata/SHA256; Blender/Pillow จำลองแสง วัสดุและฟอนต์ จึงไม่ใช่ screenshot จาก Roblox Studio

นี่เป็น development build ที่มีระบบเกมจริง โมเดลยังเป็น procedural art; PNG/audio ต้นฉบับต้องอัปโหลดและผูก asset IDs สำหรับใช้งาน imported assets และ custom skinned meshes/rigged clips ขั้นสุดท้ายยังต้องทำต่อ การเรนเดอร์จริง การเล่นบนอุปกรณ์ multiplayer และ live DataStore ยังไม่ได้ทดสอบใน Studio จากคลาวด์ Linux นี้
