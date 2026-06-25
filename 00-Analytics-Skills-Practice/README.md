# 📊 00-Analytics-Skills-Practice

ยินดีต้อนรับสู่คลังรวบรวมทักษะและการฝึกฝนด้าน **Data Analytics (DA)** โปรเจกต์ในโฟลเดอร์นี้คือรากฐานสำคัญที่ฉันใช้ในการฝึกฝนการคิดเชิงวิเคราะห์ (Analytical Thinking) การทำความสะอาดข้อมูล (Data Cleansing) และการสร้างภาพข้อมูล (Data Visualization) จนสามารถนำไปประยุกต์ใช้ในงานจริงในปัจจุบันได้สำเร็จ

---

## 🛠️ Tech Stack & Tools Used
* **Data Transformation & Cleansing:** Microsoft Excel (Advanced Formulas, Power Query)
* **Data Visualization & Modeling:** Power BI (DAX, Star Schema Data Modeling)
* **Analytical Frameworks:** Cohort Analysis, Trend Analysis, Demographic Segmentation

---

## 📂 รายละเอียดและชิ้นงานหลักในโฟลเดอร์นี้

### ☕ 1. Coffee Shop Sales & Demographic Analysis (Excel Insights)
เป็นการจำลองและวิเคราะห์ข้อมูลยอดขายของร้านเครื่องดื่ม (Coffee, Tea, Smoothie) ควบคู่ไปกับข้อมูลเชิงประชากรศาสตร์ (Demographics) เพื่อหาพฤติกรรมการซื้อของผู้บริโภคในแต่ละช่วงวัย

* **การคำนวณและแปลงข้อมูล (Data Transformation):**
  * คำนวณสัดส่วนยอดขายรายสินค้าเทียบกับผลรวมในแต่ละเดือน (% of Total) เพื่อดูการเติบโตและสัดส่วน Market Share ของสินค้าแต่ละประเภท
  * ทำระบบวิเคราะห์ผลกระทบและการเปลี่ยนแปลงของยอดขายเทียบเดือนต่อเดือน (Month-over-Month Growth & Loss Analysis) เพื่อค้นหาจุดที่ยอดขายดิ่งลงอย่างมีนัยสำคัญ
* **การแบ่งกลุ่มข้อมูลผู้บริโภค (Customer Segmentation):**
  * ใช้ฟังก์ชันจัดกรุ๊ปข้อมูลเพื่อแยกพนักงานและลูกค้าออกตามกลุ่มช่วงอายุ (Age Groups) และกลุ่ม Generation (เช่น Gen Z, Gen Y, Gen X, Baby Boomer) ทำให้ธุรกิจเข้าใจ Target Audience ได้แม่นยำยิ่งขึ้น
* **เทคนิคสูตรประยุกต์ที่ใช้:** `VLOOKUP` (Exact/Approximate Match), `XLOOKUP` สำหรับดึงข้อมูลข้ามตาราง, `SUMIF`/`COUNTIF` สำหรับสรุปยอดกลุ่มผู้ตอบแบบสอบถาม และกลุ่มสถิติต่างๆ

---

### 🧹 2. Data Cleansing & Text Manipulation Mastery
การเตรียมข้อมูล (Data Preparation) เป็นหนึ่งในทักษะที่สำคัญที่สุดของทั้ง DA และ DE ในส่วนนี้เป็นแบบฝึกหัดการจัดการกับข้อมูลประเภทข้อความ (Text) ที่ไม่มีระเบียบให้พร้อมใช้งาน

* **Case Study - Corporate Email Transformation:** * โจทย์การแปลงและสกัดโครงสร้างอีเมลจากโดเมนเก่า `@SILPAKORN.EDU` ไปเป็นโดเมนใหม่ `@su.ac.th` โดยอ้างอิงจากรหัสนักศึกษาและนามสกุลภาษาอังกฤษ
* **เทคนิคและฟังก์ชันที่ใช้:** `LEFT`, `RIGHT`, `MID`, `FIND`, และ `LEN` ร่วมกันเพื่อค้นหาตำแหน่งเครื่องหมายอักขระพิเศษ (เช่น `@` หรือ `_`) แล้วสกัดเอาเฉพาะ String ที่ต้องการออกมาสร้างเป็นคลังข้อมูลใหม่ที่มีความสะอาดและถูกต้อง 100%

---

### 🎨 3. Business Intelligence Dashboard (Power BI Project)
โปรเจกต์การเปลี่ยน Data ดิบให้กลายเป็น Interactive Dashboard เพื่อให้ฝ่ายบริหาร (Management) สามารถนำข้อมูลไปใช้ตัดสินใจทางธุรกิจได้อย่างรวดเร็ว

* **Data Modeling (Star Schema):** นำตารางข้อมูลยอดขาย (Fact Table) มาเชื่อมโยงกับตารางมิติข้อมูลต่างๆ (Dimension Tables เช่น Customers, Products, Calendars) อย่างถูกต้องเพื่อประสิทธิภาพในการ Query
* **Advanced DAX Formulas:** เขียนสูตรคำนวณวัดผล (Measures) เพื่อหา Key Performance Indicators (KPIs) ของธุรกิจ เช่น ยอดขายสะสม, อัตราการเติบโต และการเปรียบเทียบเป้าหมายการขาย
* **UI/UX Design:** ออกแบบหน้าตาแดชบอร์ดให้คลีน สแกนสายตาง่าย เลือกใช้ชาร์ตที่ตอบโจทย์กับคำถามทางธุรกิจ และควบคุมโทนสีให้ดูสบายตาและเป็นทางการ

---

## 💡 สรุปสิ่งเสร็จสิ้นและสิ่งที่ได้รับ (Key Takeaways)

1. **เข้าใจกระบวนการทำงานของข้อมูลตั้งแต่ต้นจนจบ (End-to-End Data Lifecycle):** ตั้งแต่ดึงข้อมูลดิบมาล้าง (Clean) จัดโมเดล (Model) ไปจนถึงทำภาพแสดงผล (Visualize) 
2. **สร้าง DE Mindset จากงาน DA:** การสกัดคำและแปลงรูปแบบตัวอักษรในขั้นตอนนี้ ทำให้ฉันเข้าใจถึงความสำคัญของ Data Quality และเป็นแรงผลักดันให้อยากสร้างระบบ Data Pipeline ที่เป็นอัตโนมัติ (Automation) มากยิ่งขึ้นในฝั่งของ Data Engineer

---

## 📸 ภาพตัวอย่างชิ้นงานและการวิเคราะห์

*(คำแนะนำสำหรับคุณ: สามารถนำภาพแคปหน้าจอ Dashboard สวยๆ หรือตารางวิเคราะห์ Excel ของคุณมาบันทึกไว้ในโฟลเดอร์ `assets` แล้วเรียกใช้ผ่านคำสั่งด้านล่างนี้ได้เลยค่ะ)*

### ตัวอย่างหน้าตาโมเดลและระบบวิเคราะห์ข้อมูล:
![Coffee Shop Analysis](./assets/your-excel-analysis-image.png)
![Power BI Dashboard](./assets/your-powerbi-dashboard-image.png)
