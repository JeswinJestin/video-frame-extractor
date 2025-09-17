This idea struck in my mind when I faced difficulty getting an **accurate frame** for editing, so I decided to build one.  
Here it is as a **minimum viable product (MVP)**.


# 🎬 Video Frame Extractor

This project helps extract frames from videos (YouTube, Instagram, TikTok) using **yt-dlp**, **scenedetect**, and **ffmpeg**.
It was built as a simple MVP to solve the difficulty of getting accurate frames for editing work.
A useful tool for **digital artists and video editors**.

---

## 🚀 Features

| Feature         | Description                                    |
| --------------- | ---------------------------------------------- |
| Video Download  | Downloads videos in up to **4K resolution**    |
| Scene Detection | Detects scene changes automatically            |
| FPS Extraction  | Extracts frames at fixed FPS (0.5, 1, 24, 30…) |
| Blur Removal    | Optionally skips blurry frames                 |
| Output Format   | Saves frames as a **ZIP file** for download    |

---

## 📦 Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ⚡ Usage

Run inside **Google Colab** or locally:

```bash
# Example: Extract at 24 FPS
python extractor.py --url "https://youtube.com/watch?v=xxxx" --fps 24
```

Steps in Colab:

1. Upload `cookies.txt` if the video is restricted (18+, login required).
2. Enter the video link when prompted.
3. Frames will be saved in `/frames` and zipped for download.

---

## 📂 Project Structure

```
video-frame-extractor/
│── extractor.ipynb     → Colab notebook
│── extractor.py        → Script version (optional)
│── requirements.txt    → Dependencies
│── README.md           → Project info
│── frames/             → Output frames
```

---

🎨 Example Output
```
* Extracted frames in /frames
* Scene-based cutting ensures no missed details
* Works even on age-restricted content with cookies.txt
```
🤝 Contributing

Pull requests are welcome!
For major changes, please open an issue first to discuss what you’d like to add.
 
##  Feel free to contribute. 
