# Design Patterns in C#

นี่คือ 23 Design Patterns ตามมาตรฐาน GoF ที่แบ่งออกเป็น 3 หมวดหมู่

---

## สรุปคร่าว ๆ:

- **Creational Patterns**: เน้นที่การสร้าง object ให้มีความยืดหยุ่นและควบคุมการสร้าง instance
- **Structural Patterns**: เน้นที่การจัดการการรวมกันของ object เพื่อสร้างโครงสร้างที่เหมาะสม
- **Behavioral Patterns**: เน้นที่การสื่อสารและแบ่งความรับผิดชอบในการทำงานระหว่าง object

---

## 1. Creational Patterns (การสร้าง Instance)

### 1.1 Abstract Factory
> สร้าง families ของ object ที่เกี่ยวข้องกันโดยไม่ต้องระบุคลาสที่แน่นอน

### 1.2 Builder
> แยกขั้นตอนการสร้าง object ออกจากการแสดงผล ทำให้สร้าง object ซับซ้อนได้ง่ายขึ้น

### 1.3 Factory Method
> สร้าง object โดยให้ subclass เลือกชนิด object ที่จะสร้าง

### 1.4 Prototype
> สร้าง object โดยการ clone instance ที่มีอยู่แล้ว

### 1.5 Singleton
> ทำให้ class มี instance แค่ตัวเดียวทั่วโปรแกรม

---

## 2. Structural Patterns (การจัดการโครงสร้าง)

### 2.1 Adapter
> เปลี่ยน interface ของคลาสหนึ่งให้เข้ากับอีก interface หนึ่ง

### 2.2 Bridge
> แยก abstraction กับ implementation ออกจากกันเพื่อให้สามารถพัฒนาแยกกันได้

### 2.3 Composite
> จัดการกับ object แบบ tree structure ให้เรียกใช้เหมือนกันได้ทั้ง individual และกลุ่มของ object

### 2.4 Decorator
> เพิ่ม behavior ให้กับ object แบบ dynamic โดยไม่เปลี่ยนแปลง code เดิม

### 2.5 Facade
> ให้ interface ที่ง่ายขึ้นสำหรับระบบที่ซับซ้อน

### 2.6 Flyweight
> ใช้ object reuse เพื่อลดการใช้หน่วยความจำ

### 2.7 Proxy
> ตัวแทนสำหรับ object จริง เพื่อควบคุมการเข้าถึงหรือเพิ่ม behavior ให้กับ object นั้น

---

## 3. Behavioral Patterns (การสื่อสารและควบคุมพฤติกรรม)

### 3.1 Chain of Responsibility
> ส่งต่อคำขอผ่าน chain ของ object โดยให้แต่ละ object ตัดสินใจว่าจะจัดการคำขอนั้นหรือส่งต่อไป

### 3.2 Command
> ห่อหุ้มคำสั่งเป็น object ทำให้สามารถ parameterize requests ได้

### 3.3 Interpreter
> กำหนด grammar สำหรับภาษาหนึ่ง และใช้ pattern นี้ในการตีความคำสั่ง

### 3.4 Iterator
> ให้วิธีการเข้าถึง elements ใน collection โดยไม่ต้องเปิดเผยโครงสร้างภายใน

### 3.5 Mediator
> ลดความซับซ้อนในการสื่อสารระหว่าง object ด้วยการให้ตัวกลางเป็นตัวจัดการ

### 3.6 Memento
> บันทึกและเรียกคืน state ของ object โดยไม่ทำลาย encapsulation

### 3.7 Observer
> เมื่อ object หนึ่งเปลี่ยนแปลง state แล้ว แจ้งเตือนไปยัง object อื่น ๆ ที่สนใจ

### 3.8 State
> เปลี่ยน behavior ของ object เมื่อ state ของมันเปลี่ยนไป

### 3.9 Strategy
> เปลี่ยน algorithm ในการทำงานได้แบบ runtime

### 3.10 Template Method
> กำหนดโครงสร้างขั้นตอนการทำงานโดยให้ subclass กำหนดรายละเอียดบางส่วน

### 3.11 Visitor
> เพิ่ม operation ให้กับ object โดยไม่ต้องเปลี่ยนแปลง class ของ object นั้น

---

> **หมายเหตุ:**  
> นี่คือภาพรวมของ Design Patterns ใน C# ที่สามารถใช้เป็นแนวทางในการเลือกใช้ pattern ที่เหมาะสมกับงาน
