# Git Workflow สำหรับโครงงาน ENGSE212

## ทางเลือกที่ 1: งานเล็กบน main

เหมาะกับการแก้เอกสารสั้น ๆ ที่ทีมเห็นพ้องกันแล้ว

```bash
git pull origin main
# แก้ไขไฟล์
git add <file>
git commit -m "docs(vv): update test data sheet"
git push origin main
```

## ทางเลือกที่ 2: งานบน branch + Pull Request

เหมาะกับฟีเจอร์ งานทดสอบหลายไฟล์ หรือเอกสารที่ต้อง peer review

```bash
git checkout main
git pull origin main
git checkout -b test/payment-boundary-cases
# แก้ไขไฟล์
git add .
git commit -m "test(payment): add boundary value cases"
git push -u origin test/payment-boundary-cases
```

จากนั้นเปิด Pull Request และให้เพื่อน review

## กติกาสำคัญ

- อย่า push ทับงานผู้อื่นโดยไม่ pull ล่าสุด
- ใช้ issue เชื่อมกับ defect หรือ task ที่สำคัญ
- เก็บหลักฐาน test run, screenshot และ log ใน `evidence/`
- ข้อมูลสำคัญต้องเชื่อมจาก requirement → test case → result → defect/retest
