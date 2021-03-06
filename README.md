# nozomibot

Linebot สำหรับผู้เรียนภาษาญี่ปุ่น

written in `Python 3.7` (flask) and `MySQL` (AWS RDS), deployed to [`heroku`](https://www.heroku.com)

![834majrs](https://user-images.githubusercontent.com/44984892/79058885-92a1ac00-7c9d-11ea-8600-6ed00def18ca.png)

Line ID : @834majrs

# functions

1. dictionary mode (from [JTDic](http://www.jtdic.com/2008/japanese.aspx))
    > พิมพ์คำศัพท์ภาษาญี่ปุ่นหรือคำศัพท์ไทย แล้วกดส่ง ระบบจะหาคำแปลใน JTDic (ไม่ใช่การแปลทั้งประโยค) พิมพ์ได้ทั้งคันจิและฮืรางานะ
    
    ![dic](https://user-images.githubusercontent.com/44984892/79066435-15e4f100-7ce2-11ea-9355-3434fdd88ffb.png)

2. kanji mode (ประมาณ 3000 ตัว from [Goo](https://dictionary.goo.ne.jp/kanji/) )
    > พิมพ์คำว่า "คันจิ" "kanji" หรือ "漢字" ไว้หน้าคันจิตัวเดียว แล้วกดส่ง ระบบจะแสดงวิธีอ่านและความหมาย
    >
    > เช่น "คันจิ 望"
    
    ![kanji](https://user-images.githubusercontent.com/44984892/79066450-2f863880-7ce2-11ea-8c20-39dc224820ef.png)

3. tokenization mode (โดยใช้ [`mecab-python3 0.996.5`](https://pypi.org/project/mecab-python3/))
    > พิมพ์คำว่า "ตัด" "token" "切って" หรือ "分けて" ไว้หน้าประโยคภาษาญี่ปุ่น แล้วกดส่ง ระบบจะตัดประโยคยาวๆ เป็นคำศัพท์สั้นๆ พร้อมทั้งอธิบายรูปพจนานุกรมและประเภทคำ 
    >
    > เช่น "ตัด 昨日の夜は何を食べましたか"
    
    ![token](https://user-images.githubusercontent.com/44984892/79066334-5a23c180-7ce1-11ea-8cfd-b3606a13e5ca.png)

4. conjugation mode
    > พิมพ์คำว่า "ผัน" "conj" หรือ "活用" ไว้หน้าศัพท์ที่เป็นกิริยาหรือคำคุณศัพท์ภาษาญี่ปุ่น แล้วกดส่ง ระบบจะผันคำกิริยาหรือคุณศัพท์เป็นรูปแบบต่างๆตามหลักไวยากรณ์ 
    >
    > เช่น "ผัน 行く"
    
    ![conj](https://user-images.githubusercontent.com/44984892/79066398-d5857300-7ce1-11ea-92b6-8abd042bea75.png)

5. accent mode (ประมาณ 6000 คำ from https://accent.u-biq.org/)
    > พิมพ์คำว่า "accent" หรือ "アクセント" ไว้หน้าคำศัพท์ภาษาญี่ปุ่น แล้วกดส่ง ระบบจะแสดง accent ของคำนั้น
    >
    > เช่น "accent 人形"
    
    ![accent](https://user-images.githubusercontent.com/44984892/79066417-f4840500-7ce1-11ea-8786-038f2fb866ee.png)
    
    ゆ/びに\んぎょう = ![yubiningyo](https://user-images.githubusercontent.com/44984892/79059193-4193b700-7ca1-11ea-931b-d52121fec7d2.png)
    
    accent system ของภาษาญี่ปุ่น [link (TUFS)](http://www.coelang.tufs.ac.jp/ja/th/pmod/practical/01-08-01.php)


6. wikipedia searcher
    > พิมพ์คำว่า "วิกิ" "wiki" หรือ "ウィキ" ไว้หน้าคำศัพท์ภาษาญี่ปุ่น แล้วกดส่ง ระบบจะค้นหาใน Wikipedia Japan และแสดงย่อหน้าแรก
    >
    > เช่น "วิกิ AKB48"
    
    ![wiki](https://user-images.githubusercontent.com/44984892/79066428-09609880-7ce2-11ea-8d47-6787f5363ed2.png)

7. random NHK web easy article(ประมาณ 6000 บทความ https://www3.nhk.or.jp/news/easy/)
    > พิมพ์คำว่า "NHK" แล้วกดส่ง ระบบจะสุ่มเลือกบทความจาก NHK web easy backnumbers (2013-2020)
    
    ![nhk](https://user-images.githubusercontent.com/44984892/79058948-705c5e00-7c9e-11ea-9d72-e4173b27c410.png)

# feedback & further development

หากเจอข้อผิดพลาดหรือ bug ต่างๆ กรุณารบกวนแจ้งให้ทราบโดยพิมพ์ "feedback เมสเสจ" 

หรือติดต่อทาง Facebook (ชื่อ: Nozomi Ymd) ด้วยนะครับ

ขอบคุณครับ
