# [Python - Google Sheets] Competitor & Market Analysis | Mobile Gaming

# 📊 Project Title: Competitor & Market Analysis
Author: Truong My Le  

Date: 2025-02-12

Tools Used: Python, Google Sheets 

---

## 📑 Table of Contents  

1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)
3. [📃 Main Process](#-main-process)
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)
 

---

## 📌 Background & Overview  

### Objective:

### 📖 What is this project about? What Business Question will it solve?

This project analyzes 5 competitor games in the ASMR genre to find a "Growth Formula" for our own app. It solves these business questions:

✔️ **Growth Mapping:** Who are the Top Tier, Challengers, and games at risk base on their Installs Per Day (IPD) metric và Metadata?

✔️ **Technical Correlation:** Phân tích mối tương quan giữa dung lượng App (Size) với khả năng tiếp cận người dùng, Update app versions Frequency đến hiệu suất Store.

✔️ User Feedback: What are the top complaints about competitors that we can avoid?

### 👤 Who is this project for?  

✔️ Product Owners (Định hướng lộ trình cập nhật sản phẩm).

✔️ Game Designers (Tối ưu hóa cơ chế ASMR và quảng cáo).

✔️ Marketing/UA Team (Theo dõi biến động thị trường).

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  

**Google Play Store:** Metadata and 5,000+ user reviews.

**APKPure:** Historical version dates and App Size (MB) data.

**AppStoreSpy API:** Installs Per Day (IPD) and Total Installs.


---

## 📃 Main Process

**1️⃣ Data Collection (Ad-hoc):**

- Python: Scraped metadata and user reviews from Google Play.

- Selenium: Crawled APKPure to get historical app versions and file size (MB).

- Apps Script (Google Sheets): Connected to the AppStoreSpy API to pull daily install counts (IPD) into the sheet.

**2️⃣ Growth Correlation Analysis:**

-  Mapped specific Release Dates of new versions against IPD spikes.

-  Analyzed the growth of file size over time for all 5 competitors.

-  Grouped competitors into Top Tier, Challengers, and Warning categories based on their historical stability and update consistency.

**3️⃣ Sentiment & Topic Analysis:**

- Categorized 5,000+ reviews into topics (Ad Frequency, Visual Satisfaction, ASMR Sound,...).

- Calculated Sentiment Scores (1.0 – 5.0 scale) for each topic to see what makes users positive or negative.


## 📊 Visualizations

### 1️⃣ Overview & App size

<img width="1377" height="367" alt="Screenshot 2026-03-30 174123" src="https://github.com/user-attachments/assets/5b8295ad-3048-420c-b2f4-4b14759348ae" />

<img width="1325" height="473" alt="Screenshot 2026-03-30 174155" src="https://github.com/user-attachments/assets/8e1d7dcd-284b-4036-b351-b6f7e8292238" />

### 2️⃣ Update Frequency

<img width="1162" height="405" alt="Screenshot 2026-03-30 174207" src="https://github.com/user-attachments/assets/4b969f7d-3069-4f4a-b7be-f2267f4e5272" />

<img width="1161" height="407" alt="Screenshot 2026-03-30 174217" src="https://github.com/user-attachments/assets/44fbe8cc-4e96-42f3-9645-2f93ed44f035" />

<img width="1162" height="403" alt="Screenshot 2026-03-30 174227" src="https://github.com/user-attachments/assets/e84bb3c6-34ce-42f8-b901-aa8b6fe068ec" />

<img width="1156" height="405" alt="Screenshot 2026-03-30 174236" src="https://github.com/user-attachments/assets/11f01c1a-f694-4e09-8f25-3a94cd3a53c2" />

<img width="1161" height="406" alt="Screenshot 2026-03-30 174244" src="https://github.com/user-attachments/assets/fbf2b7b5-8c23-44a9-be22-d167b7225251" />

<img width="1159" height="406" alt="Screenshot 2026-03-30 174252" src="https://github.com/user-attachments/assets/ec956fd9-072c-4c2b-a780-71907858f083" />

### 3️⃣ Topics of reviews

<img width="1082" height="334" alt="image" src="https://github.com/user-attachments/assets/9028e7b7-8f4d-42b7-90fa-a464a072cbf2" />

<img width="570" height="624" alt="Screenshot 2026-03-30 174311" src="https://github.com/user-attachments/assets/8373f883-2811-495e-9bf8-cf828d330f37" />

<img width="1173" height="446" alt="Screenshot 2026-03-30 174345" src="https://github.com/user-attachments/assets/61e1a1e9-85db-4dad-985a-fae9c844c9f2" />

## 🔎 Final Conclusion & Recommendations

📍 Market Insights & Competitor Groups:

**1️⃣ Top Tier (The Market Leaders)**

**- Home Makeover: ASMR Game:** The leader with 53M+ installs.

-> Hit a peak of 279k IPD. Success came from frequent "Micro-updates" (4 small versions in March 2025). This keeps the app in the Google Play "Recommended" section, maintaining >100k IPD.

**- House Makeover: ASMR Cleaning:** Strong performance with 17.9M+ installs and a safe 4.3 rating.

-> In late 2025, they released 8 versions keeping the size under 150MB, causing IPD to jump to 257k. However, IPD started dropping when the size exceeded 200MB in newer versions.

**2️⃣ Challengers (Potential Growth)**

**- House Cleaning ASMR:** A new app (2026).
Insight: Grew from 0 to 67,000 IPD in only 40 days by releasing 2 versions in the first month.

**- Housify: Cleaning ASMR:** 5.7M+ installs but stuck with a low 3.73 rating.
-> Despite weekly updates (12 versions in 2 months), IPD stays low (15k-30k) because the low rating discourages new users.

**3️⃣ Warning Group (High Risk)**

**- My House Makeover:** IPD is currently dropping.

-> The app size jumped to 469MB (3x larger than the old version), which immediately hurt the install rate.

📍 Recommendations:

**1. The "Size" Rule (< 200MB):**

- App Size is critical for global reach. We must optimize assets to keep the file under 200MB. Crossing this limit directly causes a drop in Daily Installs (IPD).

**2. The "Update" Strategy (Frequent & Small):**

- To trigger the Google Play algorithm, we should release 2-4 small updates per month instead of one big update every few months. This keeps the IPD stable and high.

**3. The "Rating" Threshold (> 4.0):**

- A rating below 4.0 (like Housify's 3.73) acts as a ceiling that stops growth. We must prioritize fixing bugs and reducing ad frequency to keep the rating above 4.0 before pushing for more installs.

**4. Monetization Balance:**

- Playing competitor games to map their Ad Flow, identify the "Monetization Sweet Spot" — the maximum number of ads we can show before the rating drops below the critical 4.0 threshold.
