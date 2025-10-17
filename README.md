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

🧮 Key Excel Formulas Used

| **Sheet** | **Formula** | **Description** |
|------------|-------------|-----------------|
| Transactions | `=VLOOKUP(C2,Items,2,0)` | Fetches Item Name from the Items sheet based on Item ID. |
| Transactions | `=TEXT([@Date],"MMM-YYYY")` | Converts date into Month-Year format to assist pivot grouping. |
| Invoices Detail | `=INDEX(Transactions[Date],MATCH([@[Transaction ID]],Transactions[Transaction ID],0))` | Retrieves transaction date dynamically based on matching ID. |
| Invoices Display | `=TEXTJOIN(", ",TRUE,FILTER(Invoices_Detail!$C$2:$C$201,Invoices_Detail!$A$2:$A$201=A2))` | Combines multiple customer names for the same invoice using TEXTJOIN + FILTER. |
| Invoices Display | `=TEXTJOIN(" + ",TRUE,FILTER(Invoices_Detail!$G$2:$G$201,Invoices_Detail!$A$2:$A$201=$A2)) & " = " & SUM(FILTER(Invoices_Detail!G2:G3,Invoices_Detail!A2:A3=A2))` | Summarizes total value per invoice dynamically. |
| Stock Report | `=SUMIFS(Transactions[Qty], Transactions[Item ID],[@[Item ID]], Transactions[Type],"IN")` | Calculates total incoming stock per item. |
| Stock Report | `=SUMIFS(Transactions[Qty], Transactions[Item ID],[@[Item ID]], Transactions[Type],"OUT")` | Calculates total outgoing stock per item. |
| Stock Report | `=IF([@[Current Stock]]<[@[Reorder Level]],"Low Stock","OK")` | Flags items below reorder threshold. |
| Invoice Summary | `=SUMIFS(InvoicesDetail[Line Total], InvoicesDetail[Invoice ID], [@[Invoice ID]])` | Sums all transaction values per invoice for final reconciliation. |
| Invoice Summary | `=IF([@[Total Invoice]]=[@[Total OUT]],"OK","Mismatch")` | Validates consistency between invoice total and recorded sales. |



---

📊 Project Outputs

🧱 Dashboard Overview

EN:
Summarizes warehouse performance — including sales trends, top items, and stock movements.

ID:
Menampilkan ringkasan performa gudang — mulai dari tren penjualan, barang terlaris, hingga pergerakan stok.




---

💸 Invoice Display

EN:
A complete view of the invoice template, linked to sales data and used for invoice reporting.

ID:
Tampilan lengkap template invoice yang terhubung dengan data penjualan dan disusun secara rapi untuk keperluan laporan.




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

Mockaroo and ChatGPT — For generating dummy items and transaction data



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
