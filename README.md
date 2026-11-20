# PDF Measure — วัดระยะในแบบ PDF

วัดระยะ พื้นที่ มุม เขียน markup ลายเซ็น ตราประทับ และลายน้ำบนแบบ PDF ทำงานออฟไลน์ทั้งหมด ไฟล์ไม่ถูกส่งออกจากเครื่อง

- **ใช้บนเว็บ / ติดตั้งเป็นแอป (PWA):** https://natthawat-41159.github.io/pdf-measure/
- **แอป Android (APK):** ดาวน์โหลดที่หน้า Releases ของ repo นี้ → `PDF-Measure.apk`

## ไฟล์ใน repo
| ไฟล์ | หน้าที่ |
| --- | --- |
| `index.html` | ตัวโปรแกรมทั้งหมด (ไฟล์เดียว เปิดบนคอมได้เลย) |
| `manifest.webmanifest`, `sw.js`, `icon-*.png` | ทำให้ติดตั้งเป็นแอปบนมือถือ และเปิดได้ตอนไม่มีเน็ต |
| `package.json`, `capacitor.config.json`, `assets/` | ใช้สร้างแอป Android |
| `.github/workflows/android.yml` | สั่ง GitHub สร้าง APK ให้อัตโนมัติทุกครั้งที่อัปไฟล์ใหม่ |

## อัปเดตเวอร์ชัน
แทนที่ `index.html` ด้วยไฟล์ใหม่ แล้วแก้ `VERSION` ใน `sw.js` (เช่น `pdfm-v2`) เพื่อให้มือถือโหลดเวอร์ชันใหม่ GitHub จะสร้าง APK ใหม่ให้เองภายในประมาณ 5–8 นาที
