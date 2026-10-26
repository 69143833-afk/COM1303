# COM1303
(Link)[https://github.com/69143833-afk/COM1303]
#สัปดาห์ที่ 1 โครงสร้าง HTML และแท็กพื้นฐาน 
# ผู้จัดทำ
ชื่อ-นามสกุล : ปิยวัฒน์ โกวัง
รายวิชา : COM 1303 การพัฒนาเว็บขั้นพื้นฐาน
# Git คืออะไร 
ระบบควบคุมเวอร์ชัน (Version Control System) แบบ Distributed ที่ช่วยติดตามและบันทึกการเปลี่ยนแปลงของไฟล์ในโปรเจกต์ พร้อมรองรับการทำงานร่วมกันของหลายคนอย่างเป็นระบบ ถูกสร้างโดย Linus Torvalds ในปี 2005
# การทำงานของเว็บไซต์ทำงานอย่างไร
Git แบ่งพื้นที่การทำงานเป็น 3 ส่วนหลัก:
Working Directory – พื้นที่แก้ไขไฟล์จริง
Staging Area – พื้นที่เตรียมไฟล์ก่อน Commit
Repository (.git) – ที่เก็บประวัติทั้งหมดของโปรเจกต์
# เว็บไซต์ต่างจากเว็บแอพพลิเคชั่น อย่างไร
การโต้ตอบ: เว็บไซต์โต้ตอบน้อย / เว็บแอปฯ โต้ตอบมาก
ความซับซ้อน: เว็บไซต์โครงสร้างง่าย / เว็บแอปฯ มี logic และระบบหลังบ้าน
การประมวลผล: เว็บไซต์แทบไม่มี / เว็บแอปฯ ประมวลผลทั้งฝั่งเซิร์ฟเวอร์และผู้ใช้
ฐานข้อมูล: เว็บไซต์อาจมีหรือไม่มีก็ได้ / เว็บแอปฯ ต้องมีเกือบทุกกรณี
# คู่มือการใช้งาน Github
ขั้นตอนเริ่มต้นใช้งาน GitHub
1. สมัครบัญชี GitHub
เข้าเว็บไซต์ github.com
กด Sign up
กรอกอีเมล ตั้งรหัสผ่าน และยืนยันตัวตน
เลือกแผนใช้งาน (แบบฟรีเพียงพอสำหรับผู้เริ่มต้น)
2. สร้าง Repository ใหม่
Repository คือพื้นที่เก็บโค้ดของโปรเจกต์
ขั้นตอน:
กดปุ่ม New repository
ตั้งชื่อโปรเจกต์ เช่น my-first-project
เลือกแบบ Public หรือ Private
เลือกให้สร้างไฟล์ README.md อัตโนมัติ (แนะนำ)
กด Create repository
✅ การติดตั้ง Git บนเครื่อง
Git เป็นเครื่องมือที่ใช้ร่วมกับ GitHub
Windows
ดาวน์โหลดจาก git-scm.com
ติดตั้งตามขั้นตอนมาตรฐาน
macOS
ใช้คำสั่งใน Terminal:
xcode-select --install
Linux
Ubuntu:
sudo apt install git
ตรวจสอบเวอร์ชัน:
git --version
✅ ตั้งค่าผู้ใช้งาน Git
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
✅ การเชื่อมต่อโปรเจกต์กับ GitHub
1. Clone repository ลงเครื่อง
git clone https://github.com/username/my-first-project.git
2. ตรวจสอบสถานะไฟล์
git status
3. บันทึกการเปลี่ยนแปลง (commit)
git add .
git commit -m "Initial commit"
4. ส่งโค้ดขึ้น GitHub (push)
git push origin main
5. ดึงโค้ดล่าสุดจาก GitHub (pull)
git pull origin main
✅ การทำงานร่วมกันด้วย Branch และ Pull Request
สร้าง branch ใหม่
git checkout -b feature-login
ส่ง branch ขึ้น GitHub
git push origin feature-login
สร้าง Pull Request (PR)
ไปที่หน้า repository บน GitHub
เลือกแท็บ Pull requests
กด New pull request
เลือก branch ที่ต้องการ merge
เขียนคำอธิบาย แล้วกด Create pull request
ทีมสามารถรีวิวโค้ดก่อน merge เข้าสู่ branch หลัก เช่น main
✅ การจัดการเวอร์ชันด้วย Tag และ Release
สร้าง tag
git tag v1.0.0
git push origin v1.0.0
สร้าง Release บน GitHub
ไปที่แท็บ Releases
กด Draft a new release
เลือก tag
ใส่รายละเอียดเวอร์ชัน
✅ แนวทางปฏิบัติที่ดี (Best Practices)
ใช้ commit message ให้ชัดเจน เช่น “Fix login bug”
แยกงานเป็น branch ตามฟีเจอร์
ใช้ Pull Request ทุกครั้งก่อน merge
เขียน README ให้ครบถ้วน
ใช้ .gitignore เพื่อกันไฟล์ไม่จำเป็น
✅ ตัวอย่างโครงสร้างโปรเจกต์ที่ดี
my-project/
│ README.md
│ .gitignore
│ src/
│ tests/
│ docs/
