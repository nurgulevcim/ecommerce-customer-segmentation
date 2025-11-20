# 📦 Ecommerce Customer Behavior Data Analysis

Customer segmentation and behavioral analysis using FM segmentation, discount sensitivity, channel patterns, device usage, and product category insights.

---

# ## 📘 Overview

This project explores e-commerce customer behavior to support data-driven decisions in marketing, CRM, retention, and product strategy.  
The analysis includes:

- FM scoring & segmentation  
- Discount sensitivity patterns  
- Channel usage trends (web, mobile, store)  
- Device behavior  
- Product category affinities  
- Brand loyalty patterns  
- Ads engagement  
- Social media influence  
- High-value vs. at-risk customer identification  

---

# ## 📁 Project Structure

/notebook.ipynb → Main analysis
/data/ → Dataset or link placeholder
/plots/ → Visualizations (optional)
README.md → Documentation

---

# ## 🧠 Methods Used

- Exploratory Data Analysis (EDA)  
- FM analysis & customer segmentation  
- Behavioral clustering  
- Crosstab & frequency distribution analysis  
- Correlation analysis  
- Category-level insights  

**Libraries:** pandas · numpy · matplotlib · seaborn · plotly · scikit-learn

---

# ## ❓ Key Questions

- Who are the most profitable customers?  
- Who is discount-dependent?  
- Which channels drive higher activity?  
- Which device segments have highest conversion?  
- Which categories are most preferred?  
- How do brand loyalty and ad engagement differ across segments?  
- How can marketing be personalized?

---

# ## 🔗 Dataset

Dataset source: (https://www.kaggle.com/)

---

# ## ⭐ Highlights

(These can be updated after full analysis.)

- High-value segments purchase frequently with low discount dependency.  
- Online-heavy customers show higher retention.  
- FM segmentation clearly separates customer value groups.  
- Strong category affinities visible across value tiers.  

---

# ## 🔥 **Detailed Behavioral Analysis Report (EN)**

Below is the full insight report produced after FM segmentation and behavioral analysis.

---

# # 🇺🇸 **English Version – Full Report**

---

# ## 📦 Project Overview

This project analyzes customer behavior for an e-commerce platform using **FM (Frequency–Monetary) segmentation** and multiple behavioral variables such as discount sensitivity, category preference, purchase channel, device usage, brand loyalty, ad engagement, and social media influence.

The goal was to produce **actionable customer insights** to support retention, personalization, CRM optimization, and targeted advertising.

---

# ## 🔎 FM Segmentation

Since purchase dates were unavailable, FM was used instead of RFM:

- **F (Frequency):** Number of purchases  
- **M (Monetary):** Total amount spent  

Each was quantile-scored (1–3), generating **9 FM segments**:

| Segment | Description |
|---------|-------------|
| **33** | VIP – highest-value customers |
| **32** | High spending, medium frequency |
| **31** | Loyal low-spenders |
| **23** | Lifestyle + tablet-heavy segment |
| **22** | Mixed mid-value behavior |
| **21** | Frequent, low conversion |
| **13** | Big-ticket occasional buyers |
| **12** | Promo-driven value seekers |
| **11** | Lowest-value, broad consumption |

---

# ## 🔥 Behavioral Insights

### **1️⃣ Discount Sensitivity × FM Segment**  
- Highly discount-dependent: **FM 12, FM 21, FM 22**  
- VIP (33) shows low discount dependency  
- FM 11 mixed behavior  

📊 *Plot:* `/plots/discount_sensitivity_fm.png`

---

### **2️⃣ Purchase Channel × FM Segment**
- VIP (33) → Online-heavy  
- FM 32 → Store-heavy  
- FM 12 & 13 → Omnichannel behavior  

📊 *Plot:* `/plots/purchase_channel_fm.png`

---

### **3️⃣ Device Used × FM Segment**
- VIP → Desktop-heavy (research shoppers)  
- FM 23 → Tablet-heavy  
- FM 13 → Smartphone-heavy  

📊 *Plot:* `/plots/device_fm.png`

---

### **4️⃣ Category Preferences × FM Segment**
- VIP → Electronics, Furniture, Groceries  
- FM 32 → Household categories  
- FM 23 → Clothing, Beauty, Lifestyle  
- FM 12 → Electronics + Fashion  

📊 *Plot:* `/plots/category_fm.png`

---

### **5️⃣ Brand Loyalty × FM Segment**
- Most loyal: **FM 31**  
- VIP segment shows dual behavior (loyal + disloyal split)  
- FM 23 balanced  

📊 *Plot:* `/plots/brand_loyalty_fm.png`

---

### **6️⃣ Ads Engagement × FM Segment**
- VIP → surprisingly high ad interaction  
- FM 23 → highly responsive  
- FM 11 → low-value but ad-sensitive  

📊 *Plot:* `/plots/ads_fm.png`

---

### **7️⃣ Social Media Influence × FM Segment**
- Highest influence: FM **12** and **13**  
- VIP → moderate influence  
- FM 11 → lowest influence  

📊 *Plot:* `/plots/social_media_fm.png`

---

# ## 🎯 Strategic Summary

### ✔ VIP (33)  
Prioritize premium experience, personalized recommendations, fast delivery.

### ✔ FM 23  
Ideal for influencer + digital storytelling campaigns.

### ✔ FM 12 / FM 21  
Most discount-driven → coupons, flash deals, SMS alerts.

### ✔ FM 31  
Highly loyal → cross-sell + bundle optimization.

### ✔ FM 32  
Store-oriented → offline loyalty strategy.

---

# # 🇹🇷 **Türkçe Versiyon – Detaylı Rapor**

---

# ## 📦 Proje Özeti

Bu proje, bir e-ticaret platformundaki müşteri davranışlarını analiz etmek için **FM (Frekans–Harcanan Tutar)** segmentasyonu ve çeşitli davranışsal değişkenleri kullanır. Hedef, pazarlama ve CRM süreçlerinde kullanılabilecek net ve uygulanabilir içgörüler üretmektir.

---

# ## 🔎 FM Segmentasyonu

| Segment | Açıklama |
|---------|----------|
| **33** | VIP – en yüksek değerli müşteri |
| **32** | Yüksek harcayan, orta sıklık |
| **31** | Sık alışveriş yapan sadık ama düşük harcayan |
| **23** | Tablet + lifestyle segmenti |
| **22** | Orta seviye karışık davranış |
| **21** | Sık ama düşük dönüşümlü |
| **13** | Nadiren alışveriş yapan ama yüksek tutar harcayan |
| **12** | Kampanya odaklı genç değer arayıcı |
| **11** | En düşük değer, en geniş dağılım |

---

# ## 🔥 Davranış Analizi Sonuçları

### **1️⃣ İndirim Duyarlılığı × FM**
- En promosyon odaklı: **FM 12, 21, 22**  
- VIP → düşük indirim duyarlılığı  

📊 *Grafik:* `/plots/discount_sensitivity_fm.png`

---

### **2️⃣ Alışveriş Kanalı × FM**
- VIP → online  
- FM 32 → mağaza  
- FM 12 & 13 → omnichannel  

📊 *Grafik:* `/plots/purchase_channel_fm.png`

---

### **3️⃣ Cihaz Tercihi × FM**
- VIP → Desktop  
- FM 23 → Tablet  
- FM 13 → Telefon  

📊 *Grafik:* `/plots/device_fm.png`

---

### **4️⃣ Kategori Tercihi × FM**
- VIP → Elektronik, Mobilya, Market  
- FM 23 → Lifestyle kategorileri  
- FM 12 → Elektronik + Moda  

📊 *Grafik:* `/plots/category_fm.png`

---

### **5️⃣ Marka Sadakati × FM**
- En sadık: FM 31  
- VIP → sadakat seviyesi ikiye ayrılmış  

📊 *Grafik:* `/plots/brand_loyalty_fm.png`

---

### **6️⃣ Reklam Etkileşimi × FM**
- VIP → yüksek  
- FM 23 → istikrarlı  
- FM 11 → düşük değer ama yüksek reklam duyarlılığı  

📊 *Grafik:* `/plots/ads_fm.png`

---

### **7️⃣ Sosyal Medya Etkisi × FM**
- En çok etkilenen: FM 12 ve FM 13  
- VIP → orta seviye  
- FM 11 → düşük  

📊 *Grafik:* `/plots/social_media_fm.png`

---

# ## 🎯 Stratejik Öneriler

### ✔ VIP (33)  
Premium deneyim, kişisel öneri, hızlı teslimat.

### ✔ FM 23  
Influencer + lifestyle içerikli dijital kampanyalar.

### ✔ FM 12 / 21  
Kupon, “son şans”, SMS bildirimleri.

### ✔ FM 31  
Bundle ve cross-sell stratejileri.

### ✔ FM 32  
Mağaza içi promosyonlar.

---

# ## 📝 Author

**Nurgül Evcim**  
Freelance Data Analyst – Customer Behavior & E-Commerce Insights
