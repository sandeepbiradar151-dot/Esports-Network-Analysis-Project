# 🎮 Esports Tournament Network Performance Analytics System

## 📌 Project Overview
In competitive esports, milliseconds matter. This project analyzes a telemetry dataset of **32,400 rows** to identify network bottlenecks during peak tournament hours. I engineered a statistical model to detect severe latency spikes and compared hardware performance (PC vs. Mobile) to provide data-driven infrastructure recommendations.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 🚀 Key Analysis Phases
1. **Traffic Baseline:** Identified that network latency nearly triples during evening windows (18:00–23:00).
2. **Anomaly Detection:** Used the **82nd percentile** to isolate the top **18.0% worst-case spikes** occurring above **126.5ms**.
3. **Correlation Analysis:** Mapped the direct relationship between high latency and increased packet loss percentage.
4. **Hardware Insight:** Discovered that **Mobile users** suffer a significantly higher latency penalty (119ms avg) compared to hardwired **PC users** (89ms avg) during peak loads.

## 💡 Recommendations
* **Auto-Scaling:** Implement time-based cloud server expansion starting at 17:30 on weekends.
* **Edge Computing:** Utilize localized edge nodes for mobile traffic to mitiga0te the identified 33% latency gap.