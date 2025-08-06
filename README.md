# 🧪 Product Analytics & Feature Impact Evaluation

This project evaluates user interaction with product features using a large dataset to assess **feature adoption**, **conversion funnel behavior**, and **engagement trends**. The goal is to support product decision-making by identifying key drivers of user conversion and retention.

---

## 📌 Objective

- Analyze how users interact with product features.
- Evaluate feature-level impact on conversion rates.
- Identify user segments based on device, geography, and behavior.
- Recommend product optimizations for increased engagement and conversions.

---

## 📁 Dataset

- **Name**: `product_analytics_large.csv`
- **Size**: 100,000+ records
- **Fields**:
  - `user_id`, `session_id`, `timestamp`, `device`, `country`
  - `feature_used`, `time_spent_sec`, `event_type` (`viewed`, `added_to_cart`, `purchased`)
  - `session_duration`, `features_used_count`, `converted`

---

## 🧩 Tasks Performed

### 1. Data Preparation
- Cleaned nulls, fixed types, removed duplicates.
- Engineered `conversion_funnel_stage` and `engagement_score`.

### 2. Exploratory Analysis
- Top 5 most-used product features identified.
- Conversion funnel: 100k users → 52k added_to_cart → 24k purchased.
- Drop-off rate between `added_to_cart` to `purchased`: **53%**.

### 3. Segmentation
- **Device**: Desktop users had the highest average session duration and conversions.
- **Geography**: Users from USA had highest purchase conversion; India had highest engagement time.

### 4. Impact Analysis
- Users using 3+ features were **40% more likely to convert**.
- High `time_spent_sec` correlated positively with conversions.
- Wishlist feature usage showed statistically significant impact on purchases (p < 0.01).

---

## 📊 Visualizations

- Conversion funnel visualization
- Device vs Conversion rate bar chart
- Feature usage frequency bar plot
- Heatmap: Country vs Conversion Rate

---

## 📈 Key Results

- 📌 **Feature Depth = Conversion Boost**  
  Users using 3 or more features are 40% more likely to convert.

- 📌 **Wishlist Feature Impact**  
  Using the Wishlist feature increased purchase likelihood by 22% (statistically significant).

- 📌 **Desktop = Power Users**  
  Desktop users spent 30% more time and converted 18% higher than mobile users.

---

## 🚀 Tools Used

- **Python**: pandas, seaborn, matplotlib, scipy
- **Jupyter Notebook**: analysis environment

---

## 🧠 Recommendations

- Promote high-impact features (e.g., Wishlist) more prominently.
- Optimize checkout for mobile users to reduce drop-offs.
- Target desktop-heavy users with premium recommendations.

---

## 📂 Repository Structure

