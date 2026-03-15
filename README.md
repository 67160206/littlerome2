# 👁 Littlelome AI Vision — Streamlit App

Pipeline defect detection powered by **YOLOv11** (`best.pt`)

## Detection Classes
| Class | Description |
|-------|-------------|
| `pipeline_legit` | Normal / healthy pipeline |
| `water_leak` | Water leakage detected |
| `pipe_crack` | Structural crack in pipe |
| `flame` | Fire / flame hazard |
| `corrosion` | Corrosion / rust on surface |

---

## 🚀 Deploy to Streamlit Cloud

1. Push this folder to a **GitHub repo** (include `best.pt`)
2. Go to [share.streamlit.io](https://share.streamlit.io) → **New app**
3. Select your repo, set **Main file** = `app.py`
4. Click **Deploy**

> ⚠️ `best.pt` must be in the **root of the repo** (same folder as `app.py`)

---

## 💻 Run Locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## 📁 File Structure

```
.
├── app.py                  ← Main Streamlit app
├── best.pt                 ← YOLOv11 model weights
├── requirements.txt
└── .streamlit/
    └── config.toml         ← Dark theme config
```

---

## 🗂 Features

| Tab | Feature |
|-----|---------|
| 📊 Dashboard | KPI cards, defect breakdown, system status, recent inspections |
| 📷 Live Camera | Webcam capture → instant YOLOv11 detection |
| 🖼 Upload Image | Single image analysis with annotated result download |
| 🎬 Upload Video | Frame-by-frame video analysis with timeline |
| 📋 History | Full inspection log with CSV export |
| ⚙️ Settings | Confidence threshold, alerts, class list, data management |
