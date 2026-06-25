# 📊 BI (Business Intelligence) & Data Visualization Portfolio

ยินดีต้อนรับสู่คลังรวบรวมโปรเจกต์ด้าน **Business Intelligence (BI)** โฟลเดอร์นี้รวบรวมการพัฒนาแดชบอร์ดด้วยโปรแกรม **Power BI** เพื่อแปลงข้อมูลดิบจากระบบงานขายและธุรกิจให้กลายเป็นรายงานที่มีการตอบสนองเชิงลึก (Interactive Reports) ช่วยให้ผู้บริหารและทีมงานเห็น Insight สำคัญได้ในพริบตา

---

## 🛠️ Tech Stack & Advanced Skills
* **BI Tool:** Microsoft Power BI Desktop
* **Data Connection:** Excel Workbooks, CSV Files
* **Data Modeling:** Star Schema (Fact Tables & Dimension Tables), Relationship Management (1:Many)
* **Data Transformation:** Power Query Editor (M Code, Conditional Columns, Data Cleansing)
* **Calculations:** DAX (Data Analysis Expressions) for Calculated Measures & Columns

---

## 📂 รายละเอียดโปรเจกต์ภายในโฟลเดอร์นี้

### 1. PowerBi_besic_9Expert.pbix (9Expert Sales Analytics)
โปรเจกต์สร้างรากฐานและประยุกต์ใช้โมเดลข้อมูลระดับมาตรฐานอุตสาหกรรม โดยเน้นการจัดโครงสร้างข้อมูลและการคำนวณขั้นพื้นฐานแต่ทรงพลัง
* **Data Transformation:** ใช้ Power Query ในการคลีนข้อมูล จัดประเภทประเภทข้อมูล (Data Types) ให้ถูกต้อง และรวมตารางให้อยู่ในรูปแบบที่พร้อมทำโมเดล
* **Star Schema Architecture:** เชื่อมโยงตารางมิติข้อมูล (Dimensions เช่น Customers, Products, Calendar) เข้ากับตารางข้อเท็จจริง (Fact Sales) อย่างเป็นระบบ เพื่อประสิทธิภาพในการ Query ข้อมูลความเร็วสูง
* **Key Visualizations:** การเลือกใช้ Card Visual สำหรับแสดงตัวเลข KPI สำคัญ, Stacked Bar Chart สำหรับเปรียบเทียบอันดับยอดขายสินค้า และ Line Chart สำหรับดูแนวโน้ม (Sales Trend Over Time)

### 2. Sales reports.pbix (Comprehensive Enterprise Sales Dashboard)
โปรเจกต์แดชบอร์ดวิเคราะห์ยอดขายองค์กรฉบับสมบูรณ์ ที่เน้นการออกแบบสไตล์ Dynamic Slicers และการเขียนสูตรวิเคราะห์ที่ซับซ้อนยิ่งขึ้น
* **Advanced DAX Analytics:** สร้าง Measures เพื่อคำนวณหาค่าสำคัญทางธุรกิจ เช่น ยอดขายสะสมต้นปีถึงปัจจุบัน (YTD), อัตราการเติบโตเมื่อเทียบกับช่วงเวลาเดียวกัน (YoY Growth), และการแบ่งสัดส่วนร้อยละ (% Contribution)
* **Interactive UI/UX & Slicers:** ออกแบบโครงสร้าง Dashboard ให้ใช้งานง่าย (User-Friendly) โดยมีแถบตัวกรอง (Slicers) ที่สัมพันธ์กันทั้งหมด ทั้งการกรองแยกตามภูมิภาค, แพลตฟอร์มการขาย, และทีมพนักงานขาย เพื่อให้ผู้ใช้กดเจาะลึกข้อมูล (Drill-Down) ได้ในคลิกเดียว

---

## 💡 สิ่งที่ได้เรียนรู้และตกผลึก (Key Takeaways)

1. **The Power of Data Modeling:** เข้าใจอย่างลึกซึ้งว่า แดชบอร์ดที่ดีและคำนวณได้เร็ว ไม่ได้ขึ้นอยู่กับความสวยงามเท่านั้น แต่ขึ้นอยู่กับการทำ Data Modeling (Star Schema) ที่แข็งแกร่งตั้งแต่หลังบ้าน
2. **Business Alignment:** สามารถเปลี่ยนโจทย์กว้างๆ จากฝ่ายบริหาร (เช่น "อยากรู้ว่าช่องทางไหนทำกำไรสุด") ให้กลายมาเป็น Visualizations และ Metrics (DAX) ที่ตอบโจทย์การตัดสินใจทางกลยุทธ์ได้อย่างชัดเจน

---

## 📸 ภาพตัวอย่างแดชบอร์ดภายในโปรเจกต์

*(คำแนะนำ: แนะนำให้คุณเปิดไฟล์ .pbix ทั้งสองไฟล์ แล้วแคปหน้าจอหน้า Report สวยๆ มาเก็บไว้ในโฟลเดอร์ assets เพื่อนำมาแสดงผลเป็น Portfolio ให้เห็นภาพชัดเจนที่สุดครับ)*

### ตัวอย่างหน้าตาแดชบอร์ดรายงานการวิเคราะห์:
![Power BI Sales Dashboard](./assets/your-powerbi-sales-report.png)
![Power BI Basics Insight](./assets/your-9expert-dashboard-screenshot.png)
