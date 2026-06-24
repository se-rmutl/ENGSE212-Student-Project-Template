# คู่มือการร่วมพัฒนา

## ก่อนเริ่มทำงาน

1. อ่าน issue / task ให้เข้าใจ
2. ตรวจ requirement, acceptance criteria และผลกระทบต่อการทดสอบ
3. สร้าง branch หากงานมีหลายขั้นตอนหรือกระทบไฟล์สำคัญ

## รูปแบบ branch

```text
feature/<feature-name>
fix/<bug-name>
docs/<document-name>
test/<test-scope>
```

## รูปแบบ commit

```text
docs(vv): add requirement review sheet
test(api): add order validation cases
fix(cart): prevent negative quantity
chore(repo): update project board links
```

## Pull Request

ก่อนเปิด PR ให้ตรวจ:

- [ ] Requirement และ acceptance criteria ที่เกี่ยวข้องชัดเจน
- [ ] Test cases / test result ที่เกี่ยวข้องได้รับการปรับปรุง
- [ ] ไม่มี secrets หรือข้อมูลส่วนบุคคล
- [ ] AI Use Declaration ได้รับการอัปเดต ถ้ามีการใช้ AI
- [ ] มี reviewer อย่างน้อย 1 คนเมื่อเป็นงานสำคัญ
