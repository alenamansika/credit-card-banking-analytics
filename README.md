# 💳 Credit Card Banking Analytics

## 📌 Project Overview

Proyek ini merupakan latihan analisis data credit card banking menggunakan **Google Sheets** dan **Google Looker Studio**. Dataset yang digunakan merupakan dataset credit card banking yang disediakan oleh **MySkill**, dengan informasi mengenai profil customer, aktivitas transaksi, penggunaan kartu kredit, biaya, interest, hingga delinquent account.

Dalam proyek ini, saya melakukan proses **data preparation, data transformation, data analysis, data visualization, dan dashboard development** untuk memahami karakteristik customer serta menganalisis aktivitas dan penggunaan kartu kredit dari beberapa aspek.

Dashboard dibuat secara interaktif menggunakan Google Looker Studio untuk melihat **customer demographic, customer transaction behavior, revenue profile, credit card usage, dan customer risk profile** berdasarkan beberapa dimensi seperti state, occupation, education level, marital status, dan segment.

---

## 🗂️ Dataset

- **Dataset:** Credit Card Banking Dataset
- **Source:** MySkill
- **Format:** CSV
- **Records:** 5.054
- **Columns:** 32

Dataset berisi informasi mengenai customer, transaksi, penggunaan kartu kredit, dan beberapa indikator terkait customer risk.

Beberapa informasi yang tersedia dalam dataset meliputi:

- Customer demographic
- Customer age dan gender
- Dependent count
- Education level
- Marital status
- State dan zipcode
- Car ownership dan house ownership
- Personal loan
- Customer job
- Income
- Customer satisfaction score
- Card category
- Annual fees
- Activation status
- Customer acquisition cost
- Credit limit
- Total revolving balance
- Total transaction amount
- Total transaction volume
- Average utilization ratio
- Transaction channel
- Expenditure type
- Interest earned
- Delinquent account

📎 **Dataset File:**  
`Credit Card_Dataset.csv`

---

## 🛠️ Data Preparation & Analysis

Sebelum membuat dashboard di Looker Studio, dataset terlebih dahulu dipersiapkan menggunakan **Google Sheets**.

### Data Preparation

Beberapa proses yang saya lakukan meliputi:

- Mengunggah dataset CSV ke Google Sheets
- Memeriksa struktur dan tipe data pada setiap kolom
- Melakukan transformasi data di Google Sheets
- Menyesuaikan format data sesuai kebutuhan analisis
- Memastikan data dapat digunakan sebagai Dimension maupun Metric di Looker Studio

Setelah data dipersiapkan di Google Sheets, data tersebut digunakan sebagai data source untuk membangun dashboard di Google Looker Studio.

### Data Analysis

Analisis dilakukan dari beberapa aspek utama:

- Customer demographic
- Customer transaction behavior
- Credit card usage
- Revenue profile
- Interest earned
- Customer acquisition cost
- Customer risk profile
- Delinquent account

Beberapa Dimension yang digunakan dalam analisis meliputi **state, customer job, education level, marital status, dan segment**.

Metric yang digunakan disesuaikan dengan tujuan masing-masing analisis, seperti **number of customer, transaction volume, total transaction amount, annual fees, utilization ratio, interest earned, customer acquisition cost, dan delinquent account**.

---

# 📊 Dashboard Highlights & Key Insights

## 1️⃣ Customer Demographic

Bagian ini digunakan untuk memahami karakteristik customer berdasarkan beberapa dimensi demografi.

Analisis yang ditampilkan meliputi:

- Customer by State
- Customer by Occupation
- Customer by Education
- Customer by Credit Card Experience
- Customer by Marital Status

### 🔍 Key Insight

Berdasarkan hasil analisis pada dashboard:

- **California (CA)** memiliki jumlah customer terbesar dengan **1.225 customer**.
- Berdasarkan occupation, **Selfemployeed** memiliki jumlah customer terbesar dengan **1.279 customer**.
- Berdasarkan education level, **Graduate** merupakan kelompok customer terbesar dengan **2.094 customer**.
- Berdasarkan credit card experience, **Bills** memiliki jumlah transaksi tertinggi dengan **1.482 transaksi**.
- Berdasarkan marital status, **Married** memiliki proporsi customer sebesar **51,4%**.

Analisis demographic ini digunakan untuk memberikan gambaran mengenai karakteristik customer sebelum melihat aktivitas transaksi dan credit card usage.

---

## 2️⃣ Customer Transaction & Credit Card Usage

Bagian ini digunakan untuk melihat aktivitas customer dari sisi transaksi, utilization, annual fees, dan interest earned berdasarkan occupation.

Analisis yang ditampilkan meliputi:

- Annual Fees by Occupation
- Utilization by Occupation
- Interest Earned by Occupation
- Total Transaction by Occupation

### 🔍 Key Insight

Beberapa hasil yang terlihat pada dashboard:

- **Selfemployeed** memiliki total annual fees tertinggi sebesar **370.985**.
- **Businessman** memiliki transaction volume tertinggi dengan rata-rata **80,37**.
- **Retirees** memiliki average utilization ratio tertinggi sebesar **29,22%**.
- **Businessman** memiliki total interest earned tertinggi sebesar **1.222.549,95**.

Analisis ini digunakan untuk melihat perbedaan aktivitas penggunaan kartu kredit berdasarkan occupation serta melihat indikator seperti transaction volume, utilization, annual fees, dan interest earned.

---

## 3️⃣ Revenue Generator by Segment

Analisis ini digunakan untuk melihat **Total Transaction Amount** berdasarkan customer occupation dan education level.

Pada visualisasi ini:

- **Dimension:** Customer Job
- **Breakdown Dimension:** Education Level
- **Metric:** Total Transaction Amount
- **Aggregation:** SUM

### 🔍 Key Insight

**Businessman** memiliki total transaction amount tertinggi dibandingkan occupation lainnya.

Pada kelompok Businessman, customer dengan education level **Graduate** mencatat total transaction amount sebesar **2.721.232**, diikuti oleh:

- **High School:** 1.348.635
- **Uneducated:** 1.198.605
- **Unknown:** 1.043.852
- **Doctorate:** 351.711
- **Post-Graduate:** 290.026

Analisis ini digunakan untuk melihat kontribusi transaction amount berdasarkan kombinasi occupation dan education level.

---

## 4️⃣ Customer Risk Profile

Bagian ini digunakan untuk melihat beberapa indikator yang berkaitan dengan customer risk.

Analisis yang ditampilkan meliputi:

- Customer Acquisition Cost by Occupation
- Delinquent Account by State
- Delinquent Account by Segment
- Delinquent Account by Education Level

### 🔍 Key Insight

Berdasarkan hasil pada dashboard:

- **Businessman** memiliki customer acquisition cost tertinggi sebesar **97,76**.
- **OR** memiliki persentase delinquent account tertinggi berdasarkan state.
- **Govt** memiliki delinquent account tertinggi berdasarkan segment.
- Berdasarkan education level, **Uneducated** memiliki persentase delinquent account tertinggi.

Analisis ini digunakan untuk melihat distribusi indikator delinquent account berdasarkan beberapa karakteristik customer.

> **Note:** Analisis risk profile dalam proyek ini hanya menggambarkan pola yang terdapat pada dataset dan tidak digunakan sebagai penilaian risiko aktual terhadap customer di luar dataset.

---

## 5️⃣ Customer Revenue Profile

Dashboard juga menyediakan ringkasan performa customer secara keseluruhan melalui beberapa KPI.

### 🔍 Key Insight

Berdasarkan hasil dashboard:

- **Number of Customer:** 5.054
- **Total Transaction Volume:** 326.544
- **Total Transaction Amount:** $22.314.344
- **Total Delinquent Account:** 317
- **Interest Earned:** $3.894.227
- **Avg. Cst. Satisfaction:** 11.390
- **AVG Utilization Ratio:** 27%

KPI tersebut digunakan untuk memberikan gambaran umum mengenai customer, aktivitas transaksi, transaction amount, interest earned, utilization, dan delinquent account dalam dataset.

---

# 🖼️ Dashboard Preview

![Credit Card Banking Analytics Dashboard Preview](Credit%20Card_Dashboard.jpeg)

📊 **[View Interactive Dashboard in Google Looker Studio](https://datastudio.google.com/reporting/46862dd8-a16f-4fc9-a696-c157363068b2)**

📄 **[View Full Dashboard in High-Resolution PDF](./Credit%20Card_Report.pdf)**

---

# 📁 Project Structure

**Credit Card_Dataset.csv:** Berisi dataset credit card banking yang digunakan sebagai sumber data analisis.

**Credit Card_Dashboard.jpeg:** Berisi preview dashboard.

**Credit Card_Live.pdf:** Berisi versi PDF dari dashboard yang dibuat menggunakan Google Looker Studio.

**README.md:** Berisi dokumentasi proyek, proses data preparation, analisis, key insights, dan project takeaways.

---

# 🧰 Tools & Skills Demonstrated

**Tools Used:**

- Google Sheets
- Google Looker Studio

**Skills & Techniques:**

- Data Preparation
- Data Transformation
- Dimension & Metric Configuration
- Data Aggregation
- Customer Demographic Analysis
- Transaction Analysis
- Credit Card Usage Analysis
- Revenue Analysis
- Utilization Analysis
- Interest Analysis
- Customer Acquisition Cost Analysis
- Delinquent Account Analysis
- Data Visualization
- Dashboard Development
- Data Interpretation

---

# 🎯 Project Takeaways

Melalui proyek ini, saya berlatih menganalisis data credit card banking menggunakan Google Sheets dan Google Looker Studio.

Bagian yang paling banyak saya pelajari dalam proyek ini adalah **analisis dan interpretasi data**. Dataset credit card banking memiliki banyak variabel yang saling berkaitan, sehingga saya perlu memahami konteks setiap metric dan dimension sebelum menentukan analisis yang sesuai.

Proyek ini juga membantu saya memahami bahwa pembuatan dashboard bukan hanya mengenai membuat visualisasi, tetapi juga menentukan **Dimension, Metric, dan Aggregation** yang tepat agar hasil visualisasi dapat menjawab kebutuhan analisis.

Secara keseluruhan, proses yang saya lakukan dalam proyek ini adalah:

**Raw Data → Data Preparation → Data Transformation → Data Analysis → Data Visualization → Dashboard Development → Insight**

---

# 👤 Author

**Alena Mansika**

- 💻 **GitHub:** [@alenamansika](https://github.com/alenamansika)
- 💼 **LinkedIn:** [Alena Mansika](https://www.linkedin.com/in/alenamansika)
