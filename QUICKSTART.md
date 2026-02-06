# 🚀 REDitors Voice-to-Text PRO - Quick Start Guide

## Get Professional Captions in 3 Minutes!

---

## ⚡ Super Quick Start

### 1. Install (30 seconds)

**Windows:**
```bash
Right-click install-windows.bat → Run as administrator
```

**macOS:**
```bash
sudo bash install-macos.sh
```

### 2. Configure API (1 minute)

1. Open `js/main.js` in text editor
2. Line 15: Add your OpenAI API key
```javascript
const API_KEY = 'sk-...your-key-here...';
```
3. Save file

### 3. Use Plugin (1 minute)

1. **Open Premiere Pro**
2. **Open Plugin:** `Window` → `Extensions` → `REDitors Voice-to-Text PRO`
3. **Select clip** on timeline
4. Click **"Select Audio/Video Clip"**
5. Choose **language** (or enable auto-detect)
6. Click **"Start Transcription"** (wait 10-30 seconds)
7. Click **"Create Captions"**
8. **Done!** ✨

---

## 🎯 Basic Workflow

```
Select Clip → Transcribe → Create Captions → Export (optional)
```

### Step-by-Step

1. **Clip Selection**
   - Select video/audio clip on timeline
   - Click "📌 Select Audio/Video Clip"
   - Verify clip info appears

2. **Choose Settings**
   - **Language:** Select from dropdown (or auto-detect)
   - **Model:** Whisper v1 (recommended for speed)
   - **Advanced:** Optional fine-tuning

3. **Transcribe**
   - Click "🎙️ Start Transcription"
   - Watch progress bar
   - See statistics when done

4. **Create Captions**
   - Click "✨ Create Captions"
   - Captions appear as timeline markers
   - View in Markers panel (`Window` → `Markers`)

5. **Export** (Optional)
   - **SRT:** Click "📄 Export SRT File"
   - **WebVTT:** Click "🌐 Export WebVTT"
   - **Copy:** Click "📋 Copy Full Text"

---

## 🎨 What You Get

### Sequence Markers
- ✅ Caption text in marker name
- ✅ Full text in marker comments
- ✅ Perfectly timed to audio
- ✅ Color-coded (blue)
- ✅ Visible in Markers panel

### Export Files
- ✅ **SRT** - Universal subtitle format
- ✅ **WebVTT** - Modern web format
- ✅ **Text** - Via clipboard copy

### Statistics
- ✅ Word count
- ✅ Number of segments
- ✅ Audio duration
- ✅ Processing time

---

## ⚙️ Quick Settings Guide

### Basic Settings

**Language**
- Choose your audio language
- Or enable "Auto-detect Language"

**Model**
- **Whisper v1:** Fast, accurate (recommended)
- **Whisper Medium:** Balanced
- **Whisper Large:** Most accurate

### Advanced Settings

**Auto Language Detection** 🌐
- Let AI detect language automatically
- Great for multilingual content

**Speaker Diarization** 👥
- Identifies different speakers
- Labels as [Speaker 1], [Speaker 2], etc.

**Smart Punctuation** 📝
- AI adds proper punctuation
- Better readability

**Split Long Captions** ✂️
- Auto-splits captions > 42 characters
- Better for on-screen display

**Confidence Threshold** 🎯
- Filter low-confidence words
- Higher = stricter filtering

---

## 🎬 Common Use Cases

### YouTube Video
```
1. Edit video
2. Select audio track
3. Transcribe (auto-detect or English)
4. Create captions
5. Export SRT
6. Upload video + SRT to YouTube
```

### Social Media
```
1. Short video clip
2. Transcribe with caption splitting ON
3. Create captions as markers
4. Export and style captions
5. Burn into video
6. Post to Instagram/TikTok
```

### Professional Project
```
1. Use Whisper Large model
2. Enable speaker diarization
3. Smart punctuation ON
4. Create captions
5. Export SRT
6. Import to caption track
7. Final review and delivery
```

---

## 💡 Pro Tips

### For Best Results

**🎙️ Audio Quality**
- Clean audio = better transcription
- Normalize levels first
- Remove background noise

**⚡ Speed**
- Use Whisper v1 for fastest results
- Shorter clips process faster

**🎯 Accuracy**
- Use Whisper Large for best accuracy
- Specify correct language
- Enable smart punctuation

**📊 Organization**
- Process clips in order
- Export SRT for each section
- Use markers for reference

### Keyboard Shortcuts

- `M` - Add/edit marker at playhead
- `Shift+M` - Next marker
- `Ctrl+Shift+M` - Previous marker
- `Window` → `Markers` - View all markers

---

## 🔧 Quick Troubleshooting

### Plugin Not Showing?
→ Restart Premiere Pro completely

### API Error?
→ Check your API key in main.js (line 15)

### Can't Select Clip?
→ Must be media file (not title/graphic/nested sequence)

### No Captions Created?
→ Check `Window` → `Markers` panel

### Poor Accuracy?
→ Use Whisper Large model + clean audio

---

## 📊 Supported Formats

### Input
✅ MP3, MP4, M4A, WAV, AIFF, MXF, MOV, AVI, MKV, WebM, FLAC, OGG
✅ Any format Premiere Pro supports

### Output
✅ Sequence Markers (native Premiere)
✅ SRT files
✅ WebVTT files
✅ Plain text (clipboard)

---

## 🌍 Supported Languages

🇬🇧 English | 🇪🇸 Spanish | 🇫🇷 French | 🇩🇪 German
🇮🇹 Italian | 🇵🇹 Portuguese | 🇸🇦 Arabic | 🇨🇳 Chinese
🇯🇵 Japanese | 🇰🇷 Korean | 🇷🇺 Russian | 🇮🇳 Hindi | 🇹🇷 Turkish

---

## 📝 Quick Reference

| Task | Button/Action |
|------|---------------|
| Select clip | 📌 Select Audio/Video Clip |
| Choose language | Language dropdown |
| Start | 🎙️ Start Transcription |
| Create | ✨ Create Captions |
| Export SRT | 📄 Export SRT File |
| Export WebVTT | 🌐 Export WebVTT |
| Copy text | 📋 Copy Full Text |
| View markers | Window → Markers |
| Clear log | Clear button in log panel |

---

## 🎯 What's New in v2.0

- ✨ Modern gradient UI design
- ⚡ 3 AI models (v1, Medium, Large)
- 👥 Speaker diarization
- 🌐 Auto language detection
- ✂️ Smart caption splitting
- 📊 Real-time statistics
- 🎨 Tabbed settings interface
- 📄 WebVTT export
- 🔍 Enhanced activity log
- ⏱️ Processing timer

---

## 📚 Need More Help?

### Full Documentation
See `README.md` for:
- Complete feature list
- Advanced workflows
- Detailed troubleshooting
- API configuration guide
- Best practices
- Example workflows

### Activity Log
The color-coded log shows:
- ℹ️ Info messages (blue)
- ✅ Success (green)
- ⚠️ Warnings (yellow)
- ❌ Errors (red)

Always check the log for detailed information!

---

## ⚡ One-Minute Workflow

**Fastest way to caption a video:**

1. Select clip → Click "Select"
2. Click "Start Transcription"
3. Wait for completion
4. Click "Create Captions"
5. Done!

**Captions are now on your timeline as markers!**

---

## 🎉 You're Ready!

Start creating professional captions with AI-powered transcription.

**Questions?** Check the comprehensive README.md

**REDitors Voice-to-Text PRO** - Professional tools for professional editors.

*Transform speech into perfect captions, instantly.* 🎬✨