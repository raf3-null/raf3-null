<div align="center">

# สวัสดีครับ ผม Raf3 👋

**พัฒนาแอป iOS/macOS, เว็บ และ Backend · นักศึกษามหาวิทยาลัยขอนแก่น**

ผมชอบสร้างระบบให้ครบตั้งแต่หน้าจอจนถึงฐานข้อมูลและการ deploy<br>
และมีผลงานที่ธุรกิจใช้งานจริงทุกวัน

<br>

<img src="https://skillicons.dev/icons?i=swift,kotlin,flutter,ts,nextjs,python,fastapi,spring,laravel,postgres,mysql,docker&perline=12" alt="Tech stack" />

</div>

---

## ⚡ สรุปสั้น ๆ

- 🏪 **มีผลงานใช้งานจริง** — ระบบ POS บนเดสก์ท็อปที่ธุรกิจใช้ออกใบเสร็จทุกวัน มีตัวติดตั้ง Windows และระบบอัปเดตอัตโนมัติผ่าน CI
- 🔐 **ทำงานด้านการเข้ารหัสได้** — สร้างต้นแบบส่งข้อมูลข้ามอุปกรณ์ด้วย P-256 ECDH, HKDF-SHA-256 และ AES-256-GCM พร้อม unit test
- 👥 **ทำงานเป็นทีมได้** — ร่วมพัฒนาโปรเจกต์ทีม 5–6 คน ทั้งฝั่งแอปและ Backend ทำงานผ่าน Git branch และ merge

## 🛠️ ทักษะ

| ด้าน | เทคโนโลยี |
|---|---|
| **Mobile & Desktop** | Swift, SwiftUI, CryptoKit, Kotlin, Jetpack Compose, Flutter Desktop |
| **Frontend** | TypeScript, Next.js, HTML, CSS, JavaScript |
| **Backend** | Python (FastAPI), Java (Spring Boot), PHP (Laravel) |
| **Database** | PostgreSQL, MySQL |
| **DevOps & Tools** | Docker, GitHub Actions, Vercel, Cloudflare Tunnel, Git, Figma |

---

## 🚀 ผลงานเด่น

### 🧾 ระบบ POS บนเดสก์ท็อปสำหรับธุรกิจห้องเย็น
> **สถานะ:** ใช้งานจริง · **บทบาท:** พัฒนาคนเดียวทั้งระบบ

โปรแกรมออกใบเสร็จและจัดการร้าน มาแทนโปรแกรม Python GUI ตัวเดิม

- ออกใบเสร็จ A4 หลายหน้า ตั้งค่าชื่อร้าน โลโก้ เลขผู้เสียภาษี และบัญชีธนาคารได้
- ค้นหาลูกค้าจากชื่อ ที่อยู่ เบอร์โทร หรือเลขผู้เสียภาษี และดูยอดคงเหลือของสินค้า
- รายงานยอดขายส่งออกเป็น Excel และมี Dashboard
- หน้าจอ **Flutter Desktop** ทำงานคู่กับ **Python** backend ในเครื่อง รองรับ macOS และ Windows
- ใช้ **GitHub Actions** สร้างตัวติดตั้ง Windows รัน API integration test ทดสอบติดตั้งและเปิดแอป แล้วเผยแพร่ Release ให้ระบบอัปเดตอัตโนมัติดึงไปใช้

`Flutter` `Dart` `Python` `GitHub Actions` `Inno Setup` · *Repository ไม่เปิดสาธารณะ*

### 🔐 Sendviax — ส่งข้อมูลข้ามอุปกรณ์แบบเข้ารหัส
> **สถานะ:** ต้นแบบใช้งานได้ (iOS/iPadOS, macOS, เว็บ, Relay) · **บทบาท:** ออกแบบและพัฒนาคนเดียว

ส่งข้อมูลระหว่างอุปกรณ์ของตัวเองหรือผ่านเว็บชั่วคราว โดยเข้ารหัสในเครื่องก่อนส่ง และ Relay เก็บเฉพาะข้อมูลที่เข้ารหัสแล้ว (ciphertext) ไว้ชั่วคราว

- **การเข้ารหัส:** P-256 ECDH + HKDF-SHA-256 และ AES-256-GCM ใช้ CryptoKit กับ Keychain บน Apple และ Web Crypto API บนเว็บ
- **แอป Apple:** SwiftUI สำหรับ iOS/iPadOS มี Keyboard Extension และ Share Extension และมีแอป macOS
- **Relay และเว็บ:** Relay ใช้ FastAPI ฝั่งเว็บใช้ Next.js และ deploy ด้วย Docker บนเซิร์ฟเวอร์ Windows ผ่าน Cloudflare Tunnel
- เขียนสเปกโปรโตคอลกลางไว้ให้ทุกแพลตฟอร์มใช้ร่วมกัน และมี unit test ฝั่ง Swift
- จัดทำรายงานผลประเมินความพึงพอใจของผู้ใช้
- วางแผนต่อยอดไป Android, Windows และ HarmonyOS

`Swift` `SwiftUI` `CryptoKit` `FastAPI` `Next.js` `PostgreSQL` `Docker` · *Repository ไม่เปิดสาธารณะ*

### ❄️ [ต้นแบบระบบปฏิบัติงานห้องเย็น](https://github.com/raf3-null/smit-prototype) · [ลองใช้งาน ↗](https://smit-prototype.vercel.app)
> **สถานะ:** ต้นแบบ ลองใช้ได้ทันที · **บทบาท:** พัฒนาคนเดียว

หน้าจอเปลี่ยนตามบทบาท (พนักงานขาย / คลัง / ผู้ดูแลห้องเย็น / ผู้จัดการ) บันทึกคำสั่งซื้อพร้อมระบุช่องทาง (หน้าร้าน / โทรศัพท์ / LINE / ออนไลน์) ตรวจสต็อกตามล็อต และยกเลิกพร้อมคืนสต็อกและแต้ม

*ข้อมูลเก็บในเบราว์เซอร์แต่ละเครื่อง ยังไม่มีฐานข้อมูลกลาง*

`Next.js` `TypeScript` `Vercel`

### 🏜️ DuneStock — ระบบจัดการคลังสินค้าแบบทำงานร่วมกัน
> **สถานะ:** โปรเจกต์ทีม 6 คน วิชา Mobile Device Programming · **บทบาท:** พัฒนา Android และ Backend

จัดการได้หลายคลัง เชิญทีมผ่านอีเมล แบ่งสิทธิ์ตามบทบาท (Owner / Editor / Viewer) รับเข้า-จ่ายออกพร้อมประวัติการทำงาน และสแกนบาร์โค้ด/QR

- **Android:** ระบบล็อกอินและจำสถานะการเข้าสู่ระบบ, โครงสร้าง navigation หลัก, หน้าโปรไฟล์, รวม Retrofit client ไว้ที่เดียว
- **Backend:** ออกแบบฐานข้อมูล ทำ Repository/Controller ของคลังสินค้า และแก้ปัญหา JSON วนซ้ำในความสัมพันธ์ของ Entity

`Kotlin` `Jetpack Compose` `Retrofit` `Spring Boot` `JPA` `MySQL` · *Repository ไม่เปิดสาธารณะ*

### 🏢 MyCondoCare — ระบบแจ้งซ่อมและจัดการคอนโด
> **สถานะ:** โปรเจกต์ทีม 5 คน · **บทบาท:** ร่วมพัฒนา (Laravel)

ผู้พักอาศัยแจ้งซ่อมและติดตามสถานะงานซ่อม โดยแยกหน้าจอตามบทบาท (ผู้ดูแล / เจ้าหน้าที่ / ช่าง / ผู้พักอาศัย)

`Laravel` `PHP` `Blade` · *Repository ไม่เปิดสาธารณะ*

### 🎮 [raf3 museum](https://github.com/raf3-null/raf3_museum) · [ดูเว็บ ↗](https://raf3museum.vercel.app)
เว็บคอลเลกชันอุปกรณ์เกมมิ่งโทนมืด กรองตามหมวดหมู่ และเปิดกล่องรายละเอียดด้วยคีย์บอร์ดได้ ไม่ต้อง build และไม่ใช้ไลบรารี JavaScript ภายนอก

`HTML` `CSS` `JavaScript`
