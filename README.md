# DRAGON KINGDOM TYCOON — Vivid Dragons

มังกร procedural ใหม่ครบ 20 สายพันธุ์/3 ระยะ: หัวโต ตาสองประกาย เขาโค้ง ปีกสามเหลี่ยม เกล็ดท้อง หางและเกราะร่างโต UI สีสดขอบเข้ม มีเมนูสองฝั่ง แถบทอง/เพชร/อาหาร หน้าการ์ดมังกรจริงพร้อมให้อาหาร ย้ายบ้านและจัดทีม

- [เปิดใน Roblox Studio](downloads/DragonKingdomTycoon-Vivid.rbxl)
- [Source + assets + mesh exports + คู่มือ ZIP](downloads/DragonKingdomTycoon-Vivid.zip)
- [Checksums](downloads/SHA256SUMS.txt)

หยุด Play เปิดไฟล์ Vivid ใหม่ด้วย File → Open from File แล้วกด Play รุ่นพัฒนาใช้ข้อมูลชั่วคราวเฉพาะ Studio; เกมที่เผยแพร่ใช้ DataStore เสมอ

ZIP มี Blender/FBX/OBJ/GLB และ texture ของ Mossantler Baby, Emberwing Adult, Duskveil Adult สามแบบ ต้องนำเข้าด้วย 3D Importer และ tools/dragon_mesh_import.studio.luau ตาม docs/DRAGON_MESH_IMPORT.md ก่อนใช้เป็น custom templates ในเกม เมื่อยังไม่มี template จะใช้ procedural model ใหม่ทันที ไม่มี asset IDs ที่แต่งขึ้น

ผ่าน 85 portable tests พร้อม UI/actions/responsive/portrait/world/asset checks และ Rojo build ภาพ Vivid ใน build/preview และ HeroMeshGallery ใน art/models/heroes เป็น offline renders ที่ระบุไว้ชัด ไม่ใช่ Studio screenshots

รูปทรงเป็นงานต้นฉบับตามแนว reference ยังไม่ตรงภาพ 100% งาน final ทุกสายพันธุ์/ระยะ การอัปโหลด assets, Studio import/rendering/animation และ FPS/multiplayer/live DataStore ต้องตรวจต่อบน Windows/macOS
