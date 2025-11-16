# 📥 YouTube Downloader (yt-dlp Enhanced Edition)

A powerful, modern, and user-friendly **YouTube video downloader** built using `yt-dlp` and `FFmpeg`.

This script supports:

✔ Single video downloads  
✔ Playlist downloads  
✔ Channel downloads (automatically grabs the **newest upload**)  
✔ Embedded thumbnails  
✔ Metadata injection  
✔ Duplicate prevention (download archive)  
✔ Auto-retry for unstable connections  
✔ Clean filenames  
✔ Interactive CLI prompts  

---

## 🚀 Features

### 🔹 1. Automatic Mode Detection
Just paste any URL:
- **Video URL** → downloads the video  
- **Playlist URL** → downloads the entire playlist  
- **Channel URL** → downloads the **newest uploaded video**  

### 🔹 2. Best Video Quality
Downloads:

Supports 1080p, 4K, 8K, HDR, VP9, AV1, etc.

### 🔹 3. Clean Output
- Creates download folder automatically  
- Uses safe filenames  
- Embeds thumbnails into MP4  
- Adds metadata to files  

### 🔹 4. Duplicate Prevention
The script uses `download_archive.txt` to ensure:


---

# 📦 Requirements

### 1️⃣ Python 3.8 or newer  
### 2️⃣ Install yt-dlp:
```bash
pip install yt-dlp


Ubuntu - sudo apt install ffmpeg

MACOS - brew install ffmpeg

```
### How to use

1. Run the script

2. python ytdl.py

2. Enter the YouTube URL

Examples:

https://www.youtube.com/watch?v=dQw4w9WgXcQ
https://www.youtube.com/playlist?list=PL123...
https://www.youtube.com/@LinusTechTips

3. Enter output folder

Press Enter to use default:

./downloads


Example:

Enter YouTube URL: https://www.youtube.com/watch?v=dQw4w9WgXcQ
Enter download folder (leave blank for ./downloads): D:\Videos

📁 Output Structure

Files will appear like:

downloads/
 ├─ Video Title [VIDEOID].mp4
 ├─ Video Title [VIDEOID].webp
 └─ download_archive.txt


📝 The thumbnail is embedded inside the MP4 automatically.

📌 Channel URL Behavior

If you paste a channel URL:

https://www.youtube.com/@MrBeast


The script will:

Detect it’s a YouTube channel

Retrieve the newest uploaded video

Download it immediately

This is ideal for staying up-to-date with creators.

🛑 Troubleshooting
yt-dlp not found

Install it:

pip install yt-dlp

FFmpeg errors

Ensure FFmpeg is installed and in your PATH.

Permission denied

Try saving downloads to a directory you own:

C:\Users\<you>\Videos\

Slow downloads

YouTube rate-limits sometimes — automatic retries are built in.

🧩 Customization

Inside the script, you can adjust:

Audio-only mode

Max resolution limits

Output naming

Folder organization

Playlist handling

Channel download behavior

If you want, I can generate variants like:

Audio-only MP3 downloader

Bulk downloader for multiple URLs

GUI version

Powershell .bat launcher
