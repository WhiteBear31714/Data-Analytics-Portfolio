# 🎬 Netflix Analytics Dashboard & Report

โปรเจกต์แดชบอร์ดอัจฉริยะสำหรับวิเคราะห์ข้อมูลภาพยนตร์และซีรีส์บนแพลตฟอร์ม Netflix เพื่อช่วยให้ผู้บริหารและทีมนักวิเคราะห์เนื้อหา (Content Analysts) สามารถมองเห็นแนวโน้มความนิยม พฤติกรรมของผู้ชมในแต่ละภูมิภาค และวางแผนกลยุทธ์การลงทุนซื้อลิขสิทธิ์ได้อย่างแม่นยำ

---

## 📌 Features (ฟังก์ชันการทำงานหลัก)

*   **Executive KPI Cards:** แสดงยอดสรุปทางธุรกิจที่สำคัญ เช่น ยอดวิวสะสม ทราฟฟิกประวัติ และรายรับเฉลี่ยต่อคอนเทนต์ (ARPU) 
*   **Dynamic Filtering:** ระบบตัวกรองอัจฉริยะ สามารถเลือกดูข้อมูลแยกตามภูมิภาค/ประเทศ, สตูดิโอผู้จัดทำ และหมวดหมู่ประเภทภาพยนตร์ (Genre) โดยข้อมูลบนกราฟจะอัปเดตแบบเรียลไทม์
*   **Visual Analytics Hub:** ศูนย์รวมกราฟวิเคราะห์ข้อมูลเชิงลึก
    *   *Line Chart:* แนวโน้มเวลาการรับชมรวมรายเดือน (Monthly Watch-time Trends)
    *   *Doughnut Chart:* ส่วนแบ่งตลาดผู้รับชมแยกตามพื้นที่ภูมิภาค
    *   *Bar Chart:* อันดับความนิยมของหมวดหมู่คอนเทนต์และค่ายผู้ผลิต
*   **Generative AI Insights:** เชื่อมต่อกับ **Gemini API** เพื่อวิเคราะห์ข้อมูลดิบและสร้างบทสรุปเชิงกลยุทธ์ (Content Licensing Blueprint) คาดการณ์เทรนด์คอนเทนต์ในอนาคตให้อัตโนมัติ

---

## 📊 Data Architecture (โครงสร้างข้อมูล)

โปรเจกต์นี้ขับเคลื่อนด้วยฐานข้อมูลภาพยนตร์รวมทั้งหมด **6,233 รายการ** จากไฟล์ `Netfix_report.xlsx` โดยมีการจัดเก็บแบบแยกตาราง (Relational Data Model) เพื่อประสิทธิภาพในการ Query และทำ Data Transformation:

### 1. Core Data Sheet
*   `netflix_titles`: ตารางหลักเก็บข้อมูลจำเพาะของคอนเทนต์ ประกอบด้วย รหัสคอนเทนต์ (`show_id`), ชื่อเรื่อง (`title`), ประเภท (`type`), ปีที่เข้าฉาย (`release_year`), เรตติ้งความเหมาะสม (`rating`), และคำอธิบายย่อ (`description`)

### 2. Relational Dimension Sheets (ตารางความสัมพันธ์เชิงลึก)
*   `netflix_titles_countries`: ข้อมูลประเทศหรือภูมิภาคที่คอนเทนต์นั้นเผยแพร่ (Top 5 ได้แก่ United States, India, United Kingdom, Canada, France)
*   `netflix_titles_directors`: รายชื่อผู้กำกับภาพยนตร์/ซีรีส์แต่ละเรื่อง
*   `netflix_titles_cast`: รายชื่อนักแสดงหลักที่ร่วมแสดงในคอนเทนต์นั้นๆ

### 3. Aggregated Pivot Sheets (ตารางสรุปสถิติเบื้องต้น)
*   `Pivot1`: สรุปปริมาณและสัดส่วนคอนเทนต์แยกตามประเทศ (เช่น Mexico, Germany, South Korea)
*   `Pivot2` & `Pivot3`: วิเคราะห์สัดส่วนปีที่ฉายและการกระจายตัวของเรตติ้งคอนเทนต์ (Rating Distribution) แยกตามประเภท Movie และ TV Show

---

## 🎨 UI/UX Design Theme

การออกแบบอินเตอร์เฟซยึดหลัก **Netflix Brand Configuration** เพื่อสร้างประสบการณ์การใช้งานที่ลื่นไหลและน่าดึงดูด:
*   **Theme:** Cinematic Dark Mode (พื้นหลังมืดสนิทสลับกับเส้นแสงนีออนสะท้อนโทนสีแดงอันเป็นเอกลักษณ์ของ Netflix)
*   **Clean & Scannable Layout:** จัดวางแดชบอร์ดให้สะอาดตา ไม่หนาแน่นจนเกินไป เน้นการแสดงข้อมูลที่อ่านง่าย เข้าใจได้ทันทีในพริบตา (Clarity at a glance)

---

## 🛠️ Tech Stack & Deployment

*   **Frontend:** HTML5, CSS3, JavaScript (Modern UI Component)
*   **Data Processing:** Python (Pandas, Openpyxl) / Excel Power Query
*   **AI Engine:** Gemini API (Generative Analytics Suite)
*   **Hosting/Deployment:** GitHub Pages / Firebase Hosting
