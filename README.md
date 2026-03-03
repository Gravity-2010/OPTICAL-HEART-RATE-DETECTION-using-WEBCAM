# 💓 Optical Heart Rate Detection using Webcam

A real-time, **non-contact heart rate monitoring system** that detects heart rate purely from a webcam — no wearable device required. Built as part of a university research project at Symbiosis University of Applied Sciences.

---

## 🧠 How It Works

The system detects subtle variations in **facial skin color** caused by blood circulation (rPPG — remote photoplethysmography). These color changes are imperceptible to the human eye but can be captured via webcam and analyzed using signal processing techniques.

**Pipeline:**
1. 📷 Capture live video feed via webcam
2. 🎯 Detect and isolate the face region
3. 📊 Extract RGB channel signals over time
4. 🔬 Apply **Independent Component Analysis (ICA)** to isolate the blood volume pulse signal
5. 📉 Apply **Principal Component Analysis (PCA)** for dimensionality reduction and noise filtering
6. 🌊 Use **Fast Fourier Transform (FFT)** to convert the signal to the frequency domain
7. ❤️ Identify the dominant frequency corresponding to the heart rate (BPM)

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Signal Processing | FFT, ICA, PCA |
| Computer Vision | OpenCV |
| Data & Visualization | NumPy, Matplotlib |
| Environment | Jupyter Notebook |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy opencv-python matplotlib scikit-learn jupyter
```

### Run
```bash
jupyter notebook
```
Open the main notebook and run all cells. Make sure your webcam is connected and accessible.

---

## 📌 Key Concepts

- **rPPG (Remote Photoplethysmography):** Technique to measure heart activity from skin color changes captured on camera
- **ICA:** Separates mixed signals into independent sources to isolate the pulse signal
- **FFT:** Converts time-domain signal to frequency domain to identify the heart rate frequency

---

## 👥 Contributors

Built collaboratively as part of a B.Tech final project at **Symbiosis University of Applied Sciences, Indore (2021)**.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
