# 🚦 Traffic Analyzer AI

A smart, real-time traffic monitoring web app that detects, tracks, and analyzes traffic using AI! Upload your traffic videos, and the app detects vehicles, tracks their movement, identifies congestion, flags overspeeding vehicles, and even finds cars of a specific **type** and **color**. Oh—and yes, it also gives you **cool graphs** and **downloadable reports**!

---

## 💡 What Does It Do?

Think of it like a traffic officer with AI superpowers. Here's what it does:

- 🚗 **Detects Vehicles:** Cars, trucks, bikes—you name it.
- 🎯 **Tracks Vehicles:** Follows them across frames.
- 📊 **Counts & Classifies:** Tells you how many 2-wheelers, 4-wheelers, etc.
- 🚨 **Detects Congestion & Jams:** Spots slow-moving clusters of vehicles.
- ⚡ **Flags Overspeeding:** Catches speedsters going above 120 km/h.
- 🎯 **Matches Specific Vehicles:** Looking for red trucks? It finds them!
- 📉 **Predicts Congestion:** Forecasts traffic using Machine Learning.
- 🌡️ **Generates Heatmaps:** Shows vehicle density hotspots.
- 📥 **Exports CSVs & Annotated Videos:** All reports and results are downloadable.

---

## 🛠️ Tools & Libraries Used

| Tool/Library     | Purpose |
|------------------|---------|
| **Streamlit**    | Web interface |
| **OpenCV**       | Frame processing, drawing |
| **YOLOv8 (Ultralytics)** | Vehicle detection |
| **NumPy**        | Math and arrays |
| **Pandas**       | DataFrames and CSV export |
| **Plotly**       | Interactive graphs |
| **ImageIO**      | Video output |
| **SciPy**        | Heatmap smoothing |
| **Scikit-learn** | Congestion prediction |
| **Tempfile**     | Temporary file storage |
| **OS, Time, UUID, Datetime, Collections** | System utilities |

---

## 🔍 How It Works: A Breakdown

1. **Upload Video:** MP4, AVI, MOV supported.
2. **Frame-by-Frame Analysis:**
   - YOLOv8 detects vehicles with high confidence.
   - Vehicle speeds are calculated.
   - Colors are matched using HSV ranges.
3. **Tracking:** Smart tracking with bounding boxes + path lines.
4. **Congestion & Jam Detection:**
   - Based on occupancy % and motion levels.
   - Detected using thresholds and rolling analysis.
5. **ML Prediction:** Random Forest predicts congestion for the next hour.
6. **Output:** Annotated video with overlays, CSV logs, interactive charts.

---

## 📈 Visualizations Included

- Vehicle Count vs. Time
- Traffic Jam Alerts
- Overspeeding Logs
- Congestion Level Prediction
- Live Heatmaps (Red = busy!)

---

## 📂 What Can You Download?

✅ Annotated Video (MP4)  
✅ Traffic Report CSV  
✅ Overspeeding Log  
✅ Vehicle Match Log

---

## ⚙️ Technologies & Stack

| Layer | Stack |
|-------|-------|
| UI    | Streamlit |
| AI Model | YOLOv8 (Ultralytics) |
| ML Prediction | Scikit-learn (Random Forest) |
| Video Processing | OpenCV, NumPy |
| Graphs | Plotly |
| Output Handling | Pandas, ImageIO |
| Data Smoothing | SciPy |
| Language Toggle | LangDict based |


---

## 📈 Visuals You Get

- 📊 Vehicle Count Graph (vs Time)
- 🔴 Congestion Alerts Timeline
- ⚡ Speed Distribution
- 🌡️ Real-Time Heatmap
- 📌 Detected Vehicle Snapshot
- 🗃️ CSV Reports + MP4 Annotated Videos

---

## 🔧 Benchmarks (on i5, 8GB RAM)

| Task | Avg Speed |
|------|-----------|
| Frame Processing | ~15 FPS |
| Vehicle Detection | ~0.08s/frame |
| Video Export | ~1.2x realtime |
| CSV Report Export | Instant |
| Forecast ML Model | ~1s per prediction |

---

## 🧪 Performance Tweaks

- 🟢 Confidence threshold tuning
- 🟢 Frame skipping for faster speed
- 🟢 Detection line toggling
- 🟢 Temporary vehicle tracking via UUID
- 🟢 Deprecation warnings suppressed

---

## ❓ FAQs

**Q1: Can I use my own videos?**  
✅ Yes! Just upload from your system.

**Q2: Is this real-time?**  
🕐 It works on pre-recorded videos but processes quickly enough for near-live insights.

**Q3: What happens to uploaded data?**  
🗑️ All data is processed locally and deleted from temp folders after use.

---

## 🎬 Demo Video

Watch the project in action!  
📽️ [Click here to watch the demo on YouTube](https://www.youtube.com/watch?v=YOUR_DEMO_LINK) 

---
