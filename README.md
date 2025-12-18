# Video Download & Edit

A simple, portable Windows setup for downloading videos using **yt-dlp** with **FFmpeg**.

This repository contains all required executables in a single folder so you can download and merge high‑quality video and audio without installing anything system‑wide.

---

## 📦 Contents

This folder includes:

* `yt-dlp.exe` – Video downloader
* `ffmpeg.exe` – Media processing backend
* `ffprobe.exe` – Media inspection tool
* `ffplay.exe` – Media playback tool

All executables are kept together so yt-dlp can automatically detect and use FFmpeg.

---

## 🚀 Getting Started

### 1. Open a Terminal in This Folder

In Windows Explorer:

* Right‑click inside the folder
* Select **“Open in Terminal”** (or **“Open PowerShell window here”**)

---

### 2. Download a Video

Run:

```bash
yt-dlp VIDEO_URL
```

Replace `VIDEO_URL` with the link to the video you want to download.

By default, yt-dlp:

* Downloads the **best available quality**
* Automatically merges video and audio using FFmpeg

---

### 3. Resume Interrupted Downloads

If a download fails or is interrupted, simply run the same command again:

```bash
yt-dlp VIDEO_URL
```

yt-dlp will automatically resume where it left off.

---

## ⚙️ Useful Examples

Download best video + audio (default behavior):

```bash
yt-dlp VIDEO_URL
```

Download as MP4:

```bash
yt-dlp -f "bv*+ba/b" --merge-output-format mp4 VIDEO_URL
```

Download audio only (MP3):

```bash
yt-dlp -x --audio-format mp3 VIDEO_URL
```

---

## 📁 Why This Repo Exists

* No system installation required
* No PATH configuration needed
* Easy to copy, archive, or share
* Beginner‑friendly setup for Windows users

This is intentionally minimal and portable.

---

## 🔄 Updating

To update yt-dlp:

```bash
yt-dlp -U
```

To update FFmpeg, download a newer build and replace the executables in this folder.

---

## 📜 License & Credits

* **yt-dlp**: [https://github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)
* **FFmpeg**: [https://ffmpeg.org/](https://ffmpeg.org/)

All tools are distributed under their respective licenses.

---

## ⚠️ Disclaimer

This project does **not** encourage downloading copyrighted content without permission.
Use yt-dlp responsibly and in accordance with local laws and the terms of the platforms you access.
