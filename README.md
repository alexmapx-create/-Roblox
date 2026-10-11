# DRAGON KINGDOM TYCOON — StudioFix

รุ่นแก้ไขหน้าค้างที่ “กำลังเชื่อมต่ออาณาจักร…”

- `downloads/DragonKingdomTycoon-StudioFix.rbxl`: ไฟล์เปิดใน Roblox Studio รุ่นแก้ไข
- `downloads/DragonKingdomTycoon-StudioFix.zip`: source, assets, คู่มือ, tests และไฟล์เกมทั้งชุด
- `downloads/SHA256SUMS.txt`: SHA256 ของไฟล์ดาวน์โหลด

เปิดไฟล์บน GitHub แล้วกด **Download raw file** เพื่อบันทึกลงเครื่อง จากนั้น Stop การทดสอบเดิม และ File → Open from File เพื่อเปิดไฟล์ StudioFix ก่อนกด Play

รุ่นพัฒนานี้เปิด `StudioMemoryMode = true` เฉพาะใน Studio จึงทดสอบ place ที่ยังไม่ Publish ได้ทันที HUD แจ้งว่าข้อมูลเป็นการทดสอบชั่วคราว และปิด Play แล้วข้อมูลจะหาย Published servers ใช้ DataStore จริงเสมอ หากทดสอบ save จริงใน Studio ให้ตั้ง flag false และทำตาม docs/STUDIO_SETUP.md ใน ZIP

แก้การเปิด DataStore ก่อน server พร้อมรับคำขอ, ป้องกัน bootstrap/world errors ที่ทำให้ client ค้าง, จำกัดเวลารอและคำขอที่ยังไม่ตอบ, ฟื้นตัวเมื่อ snapshot มาช้า, เว้น HUD จากปุ่ม Roblox ด้านบน และเปลี่ยนไอคอนที่เป็นตัวอักษรไม่รองรับเป็นรูปทรงเรขาคณิต

ผ่าน 75 portable tests: domain 34, security 10, persistence adapter 17, client connection 14 รวมทั้ง UI/world stand-in checks และ Rojo build ที่มี source ครบ 32 ไฟล์ สิ่งเหล่านี้เป็นการทดสอบบนคลาวด์; ยังไม่ได้ทดสอบ Studio rendering, live DataStore, multiplayer และ FPS จริง

ถ้าต้องการดูข้อความผิดพลาด เปิด Window (หน้าต่าง) → Output ใน Studio รุ่นใหม่; รุ่นเก่าใช้ View → Output

Artwork/audio ต้นฉบับยังต้องอัปโหลดและผูก asset IDs โดยเจ้าของ โมเดลมังกร procedural เป็นงานพัฒนาที่รอ custom meshes/rigged clips ขั้นสุดท้าย ที่มา assets อยู่ใน art/LICENSE.md ใน ZIP ไม่ได้ประกาศ source เป็น open source
