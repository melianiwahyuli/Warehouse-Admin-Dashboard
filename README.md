🧮 Warehouse Dashboard Project

(English + Bahasa Indonesia)




---

📋 Project Overview

EN:
This project demonstrates how Microsoft Excel can function as a complete warehouse management and business analytics tool — without using any macros or code.
It integrates datasets, reports, and interactive dashboards into one file, showing how data can be transformed into insights through formulas, pivot tables, and visualization.

ID:
Proyek ini menunjukkan bagaimana Microsoft Excel dapat digunakan sebagai alat manajemen gudang dan analisis bisnis yang lengkap — tanpa makro atau pemrograman.
Semua data, laporan, dan dashboard interaktif digabung dalam satu file, memperlihatkan bagaimana data mentah dapat diubah menjadi insight dengan formula, pivot table, dan visualisasi.


---

🗂️ Dataset & Files

📘 Main File: Warehouse Admin Project by Meliani Wahyuli.xlsx

EN:
This single Excel file contains the entire workflow:

Raw dataset (items, transactions, invoices)

Processed data tables

Final dashboards and KPI summaries


ID:
File Excel ini mencakup seluruh proses kerja:

Data mentah (barang, transaksi, dan invoice)

Data hasil olahan

Dashboard akhir dan ringkasan KPI



---

📊 Project Outputs

🧱 Dashboard Overview

EN:
Summarizes warehouse performance — including sales trends, top items, and stock movements.
ID:
Menampilkan ringkasan performa gudang — mulai dari tren penjualan, barang terlaris, hingga pergerakan stok.




---

📜 Stock Report

EN:
Displays real-time stock levels and low-stock alerts automatically after each transaction.
ID:
Menunjukkan stok terkini secara otomatis dan memberikan peringatan barang yang perlu restock.




---

🧾 Invoice Summary

EN:
Summarizes all invoices and reconciles sales transactions dynamically.
ID:
Menyajikan rekap invoice serta pengecekan otomatis antara data penjualan dan transaksi.




---

💸 Invoice Display

EN:
Full invoice layout automatically linked to sales and customer data.
ID:
Tampilan penuh template invoice otomatis yang terhubung dengan data penjualan dan pelanggan.




---

🔢 Core Formulas Used

EN:
The following Excel functions were used throughout the project to automate calculations, validate data, and link tables dynamically.
ID:
Berikut formula utama yang digunakan untuk otomatisasi perhitungan, validasi data, dan penghubung antar tabel.

Category	Formula	Description

Stock Movement	=SUMIFS(Transactions[Qty], Transactions[Item ID],[@[Item ID]], Transactions[Type],"IN")	Calculates total stock IN per item
	=SUMIFS(Transactions[Qty], Transactions[Item ID],[@[Item ID]], Transactions[Type],"OUT")	Calculates total stock OUT per item
Current Stock	=Items[@Stock]+[@[Total IN]]-[@[Total OUT]]	Updates real-time stock level
Low Stock Alert	=IF([@Current Stock]<[@Reorder Level],"Low Stock","OK")	Highlights items that need restocking
Invoice Reconciliation	=IF([@[Total Invoice]]=[@[Total OUT]],"OK","Mismatch")	Validates data consistency between invoice & sales
Month-Year Grouping	=TEXT([@Date],"MMM-YYYY")	Groups transactions by month for trend charts
Customer Summary	=TEXTJOIN(", ",TRUE,FILTER(Transactions[Customer],Transactions[Invoice]=[@Invoice]))	Auto-list of customers per invoice
Sales Trend	=SUMIFS(Sales[Amount],Sales[Month],[@Month])	Aggregates monthly revenue for dashboard visuals



---

🧠 Key Insights

EN:

📆 Highest monthly sales: July 2025

💰 Best-performing category: Electronics

📊 Real-time stock updates per transaction

🧮 Fully automated formulas across all sheets


ID:

📆 Penjualan tertinggi terjadi pada Juli 2025

💰 Kategori dengan performa terbaik: Elektronik

📊 Stok otomatis terupdate setiap transaksi

🧮 Semua formula bekerja otomatis di seluruh sheet



---

⚙️ Tools Used

Microsoft Excel — Main analytics & visualization tool

Canva / Snipping Tool — For dashboard and report previews

(Optional) Mockaroo — For generating dummy transaction data



---

🧑‍💻 Skills Demonstrated

EN:

Data cleaning & transformation

PivotTables & dashboard design

Conditional formatting

Advanced Excel formulas (VLOOKUP, SUMIFS, TEXTJOIN, FILTER)

Analytical storytelling & layout design


ID:

Pembersihan & transformasi data

Desain PivotTable & dashboard interaktif

Conditional formatting untuk insight visual

Formula Excel lanjutan (VLOOKUP, SUMIFS, TEXTJOIN, FILTER)

Penyajian data secara analitis & desain layout profesional



---

🏁 Repository Structure

📁 Warehouse-Dashboard-Project/
├── 📘 Warehouse Admin Project by Meliani Wahyuli.xlsx
├── 📘 Dashboard_Report.pdf
├── 🖼️ dashboard_preview.png
├── 🖼️ invoices_display.png
├── 🖼️ stock_report.png
├── 🖼️ invoice_summary.png
├── 🖼️ formulas_preview.png
└── 📘 README.md


---

💬 Author

Meliani Wahyuli [Meli]
📍 Excel & Data Enthusiast | Warehouse Data Analyst (Simulation)
📧 wahyulimeliani@gmail.com

> “Data is silent — Excel helps it speak.”
