# ใบงานการทดลอง HTML

## การทดลองที่ 5: การสร้างตารางและรายการ
### วัตถุประสงค์
- เรียนรู้การสร้างตารางข้อมูล
- เรียนรู้การสร้างรายการแบบต่างๆ

### ขั้นตอนการทดลอง
1. สร้างไฟล์ tablelist.html ดังตัวอย่าง:
```html
<table border="1">
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
        </tr>
    </tbody>
</table>
```

### คำอธิบายเพิ่มเติม
- `<table>` กำหนดขอบเขตของตาราง
- `<thead>` สำหรับส่วนหัวตาราง
- `<tbody>` สำหรับเนื้อหาตาราง
- `<tr>` แทนแถว
- `<th>` แทนเซลล์หัวตาราง
- `<td>` แทนเซลล์ข้อมูล

2. การสร้างรายการ โดยเพิ่มเติม Code ในไฟล์ tablelist.html :
```html
<ul>
    <li>Unordered item 1</li>
    <li>Unordered item 2</li>
</ul>

<ol>
    <li>Ordered item 1</li>
    <li>Ordered item 2</li>
</ol>

<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```

### คำอธิบายเพิ่มเติม
- `<ul>` สำหรับรายการแบบไม่เรียงลำดับ
- `<ol>` สำหรับรายการแบบเรียงลำดับ
- `<dl>` สำหรับรายการแบบคำจำกัดความ
- `<li>` แทนรายการแต่ละรายการ

### แบบฝึกหัด
1. สร้างตารางแสดงข้อมูลส่วนตัว
2. สร้างรายการเมนูอาหาร

[วางโค้ด HTML ที่นี่]
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Table</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 0;
            background-color: #f9f9f9;
        }
        table {
            width: 50%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: center;
        }
        .menu-item {
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ddd;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .menu-item h3 {
            margin: 0 0 5px;
            font-size: 1.2rem;
        }
        .menu-item p {
            margin: 0;
            color: #666;
        }
    </style>
</head>
<body>

    <h1>ข้อมูลส่วนตัว</h1>
    <table>
        <thead>
            <tr>
                <th>หัวข้อ</th>
                <th>ข้อมูล</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>ชื่อ</td>
                <td>จณิศตา ดีศรี</td>
            </tr>
            <tr>
                <td>ชื่อเล่น</td>
                <td>จอนอ</td>
            </tr>
            <tr>
                <td>อายุ</td>
                <td>19 ปี</td>
            </tr>
            <tr>
                <td>อาชีพที่อยากเป็นในอนาคต</td>
                <td>ครู</td>
            </tr>
            <tr>
                <td>มหาวิทยาลัย</td>
                <td>สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง</td>
            </tr>
            <tr>
                <td>คณะ</td>
                <td>คณะครุศาสตร์อุตสาหกรรมและเทคโนโลยี</td>
            </tr>
            <tr>
                <td>สาขาวิชา</td>
                <td>เทคโนโลยีคอมพิวเตอร์</td>
            </tr>
        </tbody>
    </table>

    <h1>เมนูอาหาร</h1>
    <div class="menu-item">
        <h3>กุ้งทอด</h3>
        <p>ราคา: 17 บาท</p>
    </div>
    <div class="menu-item">
        <h3>เกี๋ยวหมูทอด</h3>
        <p>ราคา: 12 บาท</p>
    </div>
    <div class="menu-item">
        <h3>ขนมจีบ</h3>
        <p>ราคา: 16 บาท</p>
    </div>
    <div class="menu-item">
        <h3>ไก่ทอด</h3>
        <p>ราคา: 15 บาท</p>
    </div>
    <div class="menu-item">
        <h3>หมูทอด</h3>
        <p>ราคา: 12 บาท</p>
    </div>
    <div class="menu-item">
        <h3>เห็ดเข็มทองทอด</h3>
        <p>ราคา: 15 บาท</p>
    </div>
    <div class="menu-item">
        <h3>สาหร่ายทอด</h3>
        <p>ราคา: 10 บาท</p>
    </div>
    <div class="menu-item">
        <h3>ปลาทอด</h3>
        <p>ราคา: 5 บาท</p>
    </div>

</body>
</html>
```
- ภาพผลลัพธ์:
[วางภาพ screenshot ที่นี่]

<img width="1470" alt="Screenshot 2568-02-06 at 00 34 25" src="https://github.com/user-attachments/assets/a796ead3-efe8-499d-8fd1-edf6b2d19740" />
![Uploading Screenshot 2568-02-06 at 00.34.35.png…]()
