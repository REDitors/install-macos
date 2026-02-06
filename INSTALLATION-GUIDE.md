# 🎬 REDitors Voice-to-Text PRO - Complete Installation & Usage Guide

## 📦 Package Contents

You have received a complete, production-ready Adobe Premiere Pro plugin with:

- ✅ All core files properly organized
- ✅ Automated installation scripts
- ✅ Comprehensive documentation
- ✅ Bug fixes and optimizations applied
- ✅ Professional gradient UI
- ✅ Advanced AI features

---

## 🚀 QUICK START (3 Steps)

### 1️⃣ INSTALL (2 minutes)

**Windows:**
```
1. Right-click install-windows.bat
2. Select "Run as administrator"
3. Wait for completion
```

**macOS:**
```bash
1. Open Terminal
2. Navigate to plugin folder
3. Run: sudo bash install-macos.sh
4. Enter your password
```

### 2️⃣ CONFIGURE (1 minute)

**Add Your OpenAI API Key:**

After installation, edit this file:
- **Windows:** `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro\js\main.js`
- **macOS:** `/Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/js/main.js`

Find line 15 and replace with YOUR API key:
```javascript
const API_KEY = 'sk-YOUR-ACTUAL-OPENAI-API-KEY-HERE';
```

**Don't have an API key?**
1. Go to: https://platform.openai.com/api-keys
2. Sign up/log in
3. Click "Create new secret key"
4. Copy the key (starts with `sk-`)
5. Add credits: https://platform.openai.com/account/billing

### 3️⃣ USE (30 seconds)

```
1. Restart Premiere Pro completely
2. Open plugin: Window → Extensions → REDitors
3. Select clip on timeline
4. Click "Select Audio/Video Clip"
5. Click "Start Transcription"
6. Click "Create Captions"
7. Done! ✨
```

---

## 📁 What's Inside the Package

```
REDitors-VoiceToText-PremierePro/
│
├── 📘 START-HERE.md           ← Read this first!
├── 📗 SETUP-GUIDE.md          ← Detailed installation
├── 📙 QUICKSTART.md           ← Quick reference
├── 📕 README.md               ← Full documentation
├── 📔 PLUGIN-STATUS.txt       ← Status & checklist
│
├── 🔧 install-windows.bat     ← Windows installer
├── 🔧 install-macos.sh        ← macOS installer
│
├── 📂 CSXS/
│   └── manifest.xml           ← Plugin configuration
│
├── 📂 js/
│   ├── main.js                ← ⚠️ ADD API KEY HERE (line 15)
│   └── libs/
│       └── CSInterface.js     ← Adobe CEP library
│
├── 📂 jsx/
│   └── hostscript.jsx         ← Premiere Pro integration
│
├── 📂 icons/
│   └── icon-info.txt          ← Icon info
│
├── 🌐 index.html              ← User interface
├── 🔍 .debug                  ← Debug configuration
└── 📄 package.json            ← Plugin metadata
```

---

## ⚙️ Detailed Installation Instructions

### Windows Installation

**Step 1: Run Installer**
```
1. Locate install-windows.bat in the plugin folder
2. RIGHT-CLICK the file
3. Select "Run as administrator"
4. Click "Yes" on the security prompt
5. Wait for "Installation Successful!" message
6. Press any key to close
```

**Step 2: Verify Installation**
```
Navigate to:
C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\

You should see:
REDitors-VoiceToText-PremierePro\
```

**Step 3: Configure API Key**
```
1. Navigate to:
   C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro\js\

2. Right-click main.js → Open with → Notepad (or Notepad++)

3. Find line 15:
   const API_KEY = 'sk-proj-ijCUSQ...';

4. Replace with YOUR API key:
   const API_KEY = 'sk-YOUR-KEY-HERE';

5. Save the file (Ctrl+S)
6. Close the editor
```

**Step 4: Enable Debug Mode (if needed)**
```
1. Press Win+R
2. Type: regedit
3. Navigate to: HKEY_CURRENT_USER\Software\Adobe\CSXS.11
4. Right-click → New → String Value
5. Name: PlayerDebugMode
6. Value: 1
7. Close Registry Editor
```

### macOS Installation

**Step 1: Run Installer**
```bash
1. Open Terminal (Applications → Utilities → Terminal)

2. Navigate to plugin folder:
   cd /path/to/REDitors-VoiceToText-PremierePro

3. Run installer:
   sudo bash install-macos.sh

4. Enter your password when prompted

5. Wait for "Installation Successful!" message
```

**Step 2: Verify Installation**
```bash
Navigate to:
/Library/Application Support/Adobe/CEP/extensions/

You should see:
REDitors-VoiceToText-PremierePro/
```

**Step 3: Configure API Key**
```bash
1. Open Terminal

2. Edit main.js:
   sudo nano "/Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/js/main.js"

3. Find line 15 (use arrow keys to navigate):
   const API_KEY = 'sk-proj-ijCUSQ...';

4. Replace with YOUR API key:
   const API_KEY = 'sk-YOUR-KEY-HERE';

5. Save: Ctrl+O, Enter
6. Exit: Ctrl+X
```

**Or use TextEdit:**
```
1. Open TextEdit
2. File → Open
3. Navigate to: /Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/js/main.js
4. Edit line 15 with your API key
5. Save
```

**Step 4: Enable Debug Mode (if needed)**
```bash
defaults write com.adobe.CSXS.11 PlayerDebugMode 1
```

---

## 🔑 Getting Your OpenAI API Key

### Step-by-Step

1. **Create Account**
   - Go to: https://platform.openai.com
   - Click "Sign up" (or "Log in" if you have account)
   - Complete registration

2. **Generate API Key**
   - Go to: https://platform.openai.com/api-keys
   - Click "Create new secret key"
   - Give it a name (e.g., "Premiere Pro Plugin")
   - Click "Create secret key"
   - **IMPORTANT:** Copy the key immediately (starts with `sk-`)
   - You won't be able to see it again!

3. **Add Credits**
   - Go to: https://platform.openai.com/account/billing
   - Click "Add payment method"
   - Add credit card
   - Add credits (minimum $5 recommended)
   - Credits don't expire!

4. **Verify Setup**
   - Go to: https://platform.openai.com/usage
   - You should see your usage dashboard
   - Ready to use!

---

## 💰 Cost Breakdown

### Plugin Cost
**FREE** - You already have it!

### API Usage Cost
Based on OpenAI Whisper API pricing:

**~$0.006 per minute of audio**

**Examples:**
- 10 minutes of audio = $0.06
- 30 minutes of audio = $0.18
- 1 hour of audio = $0.36
- 10 hours of audio = $3.60

**Very affordable for professional use!**

### Recommended Starting Credits
- **$5-10** for testing and small projects
- **$20-50** for regular professional use
- **$100+** for heavy usage

You only pay for what you use!

---

## 🎯 Using the Plugin

### First Time Setup

1. **Open Premiere Pro**
   - Start Adobe Premiere Pro
   - Open a project with a sequence

2. **Open Plugin Panel**
   - Go to: **Window → Extensions**
   - Look for: **REDitors** or **REDitors Voice-to-Text PRO**
   - Click to open panel

3. **Verify Plugin Loaded**
   - Panel should display modern gradient interface
   - See "REDitors Voice-to-Text PRO" header
   - Activity log visible at bottom

### Basic Workflow

**Step 1: Select Clip**
```
1. Place a video/audio clip on timeline
2. Select the clip (click on it)
3. In plugin, click "📌 Select Audio/Video Clip"
4. Verify clip info appears
```

**Step 2: Configure Settings**
```
Basic Settings:
- Language: Choose from dropdown (or enable auto-detect)
- Model: Whisper v1 (recommended for speed)

Advanced Settings (optional):
- Auto Language Detection
- Speaker Diarization
- Smart Punctuation
- Split Long Captions
```

**Step 3: Transcribe**
```
1. Click "🎙️ Start Transcription"
2. Watch progress bar
3. Wait for completion (typically 10-30 seconds)
4. Review statistics in results panel
```

**Step 4: Create Captions**
```
1. Click "✨ Create Captions"
2. Captions added as sequence markers
3. View in: Window → Markers panel
4. Markers show on timeline
```

**Step 5: Export (Optional)**
```
- SRT File: Click "📄 Export SRT File"
  (Saves to Desktop as SequenceName.srt)

- WebVTT: Click "🌐 Export WebVTT"
  (Saves to Desktop as SequenceName.vtt)

- Copy Text: Click "📋 Copy Full Text"
  (Copies transcription to clipboard)
```

---

## 🎨 Features Explained

### AI Models

**Whisper v1** (Default)
- Fast processing
- High accuracy
- Recommended for most use cases
- Best for: Quick turnaround projects

**Whisper Medium**
- Balanced speed/accuracy
- Good for complex audio
- Best for: Professional projects

**Whisper Large**
- Highest accuracy
- Slower processing
- Best for: Critical professional work, difficult audio

### Language Support

🇬🇧 English | 🇪🇸 Spanish | 🇫🇷 French | 🇩🇪 German  
🇮🇹 Italian | 🇵🇹 Portuguese | 🇸🇦 Arabic | 🇨🇳 Chinese  
🇯🇵 Japanese | 🇰🇷 Korean | 🇷🇺 Russian | 🇮🇳 Hindi | 🇹🇷 Turkish

**Auto-Detect:** Let AI determine language automatically

### Advanced Features

**Speaker Diarization** 👥
- Identifies different speakers
- Labels as [Speaker 1], [Speaker 2], etc.
- Great for interviews, podcasts

**Smart Punctuation** 📝
- AI adds proper punctuation
- Improves readability
- Professional results

**Smart Caption Splitting** ✂️
- Auto-splits captions over 42 characters
- Better for on-screen display
- Follows best practices

**Confidence Filtering** 🎯
- Filter low-confidence words
- Threshold: 0-100%
- Higher = stricter filtering

---

## 🛠️ Troubleshooting

### Plugin Not Showing?

**Solution 1: Restart Premiere Pro**
```
1. Close ALL Premiere Pro windows
2. Wait 10 seconds
3. Reopen Premiere Pro
4. Check Window → Extensions → REDitors
```

**Solution 2: Enable Debug Mode**

Windows:
```
1. Win+R → regedit
2. Navigate to: HKEY_CURRENT_USER\Software\Adobe\CSXS.11
3. Create String Value: PlayerDebugMode = 1
4. Restart Premiere Pro
```

macOS:
```bash
defaults write com.adobe.CSXS.11 PlayerDebugMode 1
# Restart Premiere Pro
```

**Solution 3: Verify Installation**
```
Check that files exist at:
Windows: C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro\
macOS: /Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/
```

### API Errors

**"Invalid API Key"**
```
1. Open js/main.js
2. Check line 15 has your real API key
3. Key should be in quotes: 'sk-...'
4. Verify key at: platform.openai.com/api-keys
5. Make sure you saved the file!
```

**"Insufficient Credits"**
```
1. Go to: platform.openai.com/account/billing
2. Add payment method
3. Add credits ($5 minimum recommended)
4. Wait a few minutes
5. Try again
```

**"Network Error"**
```
1. Check internet connection
2. Try again in a moment
3. OpenAI API might be temporarily down
4. Check status: status.openai.com
```

### Can't Select Clip

**Requirements:**
- ✅ Must be imported media file
- ✅ Must be selected on timeline
- ✅ Must have audio
- ✅ Must be in active sequence

**Won't Work With:**
- ❌ Titles or graphics
- ❌ Nested sequences
- ❌ Adjustment layers
- ❌ Clips in bin (not on timeline)

### No Captions Created

**Check:**
1. Window → Markers panel (captions are markers)
2. Activity Log in plugin for errors
3. Make sure transcription completed successfully
4. Try a shorter clip first (10-20 seconds)
5. Check sequence is active

---

## 💡 Pro Tips

### For Best Results

**Audio Quality**
- Clean audio = better transcription
- Normalize audio levels first
- Remove background noise if possible
- Use best quality audio available

**Model Selection**
- Quick projects → Whisper v1
- Professional work → Whisper Large
- Balanced needs → Whisper Medium

**Language Settings**
- Specify language when possible
- Auto-detect good for multilingual
- Better accuracy with specified language

**Workflow Optimization**
- Process clips in order
- Export SRT for archiving
- Use markers for quick reference
- Import SRT to caption track for final edit

### Keyboard Shortcuts (Premiere Pro)

```
M              - Add marker at playhead
Shift+M        - Go to next marker
Ctrl+Shift+M   - Go to previous marker
```

### Export Best Practices

**For YouTube/Social Media:**
- Export SRT file
- Upload video + SRT separately
- Let platform handle styling

**For Professional Delivery:**
- Export SRT
- Import to caption track
- Review and edit captions
- Style as needed
- Export with burned-in captions

---

## 📊 Supported Formats

### Input (Audio/Video)
✅ MP3, MP4, M4A, WAV, AIFF  
✅ MXF, MOV, AVI, MKV, WebM  
✅ FLAC, OGG  
✅ Any format Premiere Pro supports

### Output
✅ Sequence Markers (Premiere Pro native)  
✅ SRT subtitle files (.srt)  
✅ WebVTT files (.vtt)  
✅ Plain text (clipboard)

---

## ✅ Installation Checklist

### Before Installation
- [ ] Adobe Premiere Pro 2020+ installed
- [ ] Have admin/sudo access
- [ ] Downloaded plugin package
- [ ] Extracted all files
- [ ] Read this guide

### During Installation
- [ ] Ran installer as admin/sudo
- [ ] Installation completed successfully
- [ ] No error messages
- [ ] Files copied to correct location

### After Installation
- [ ] Obtained OpenAI API key
- [ ] Edited js/main.js with API key
- [ ] Saved the file
- [ ] Added credits to OpenAI account
- [ ] Restarted Premiere Pro completely

### Verification
- [ ] Plugin appears in Extensions menu
- [ ] Panel opens without errors
- [ ] Can select clip on timeline
- [ ] Transcription works
- [ ] Captions created successfully

---

## 📞 Support & Resources

### Documentation Files
- **START-HERE.md** - Quick overview
- **SETUP-GUIDE.md** - This file
- **QUICKSTART.md** - Daily usage reference
- **README.md** - Complete feature documentation
- **BUGFIX.md** - Known issues and solutions
- **PLUGIN-STATUS.txt** - Status checklist

### Online Resources
- **OpenAI Platform:** https://platform.openai.com
- **API Documentation:** https://platform.openai.com/docs
- **API Keys:** https://platform.openai.com/api-keys
- **Billing:** https://platform.openai.com/account/billing
- **Status:** https://status.openai.com

---

## 🎓 Learning Resources

### Day 1: Getting Started
1. Install plugin (10 minutes)
2. Configure API key (5 minutes)
3. First transcription (5 minutes)
4. Create first captions (2 minutes)
**Total: ~30 minutes**

### Day 2: Basic Features
1. Try different languages
2. Test different models
3. Practice caption creation
4. Export SRT files
**Total: ~1 hour**

### Day 3: Advanced Features
1. Speaker diarization
2. Smart punctuation
3. Caption splitting
4. Workflow optimization
**Total: ~1-2 hours**

### Week 1: Master It
- Process real projects
- Optimize your workflow
- Learn keyboard shortcuts
- Build efficiency

---

## 🎬 Example Workflows

### YouTube Video
```
1. Edit video in Premiere
2. Select audio track
3. Transcribe (Whisper v1, English)
4. Create captions
5. Export SRT
6. Upload to YouTube with SRT
```

### Social Media (Instagram/TikTok)
```
1. Edit short video
2. Select clip
3. Transcribe with caption splitting ON
4. Create captions
5. Review markers
6. Burn into video
7. Export final video
```

### Professional Documentary
```
1. Edit rough cut
2. Select interview clips
3. Transcribe (Whisper Large, specific language)
4. Speaker diarization ON
5. Create captions
6. Export SRT
7. Import to caption track
8. Professional review/edit
9. Final delivery
```

### Podcast Episode
```
1. Import audio
2. Create sequence
3. Select full audio
4. Transcribe with speaker ID
5. Create markers
6. Export SRT for show notes
7. Copy text for blog post
```

---

## 🔄 Update Instructions

If a new version is released:

1. **Backup Current Version**
   ```
   Copy your current installation folder
   Save your API key separately
   ```

2. **Uninstall Old Version**
   ```
   Delete the plugin folder from:
   Windows: C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro\
   macOS: /Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/
   ```

3. **Install New Version**
   ```
   Run new installer
   Add API key
   Restart Premiere Pro
   ```

---

## ⚠️ Important Notes

### API Key Security
- ❌ Never share your API key
- ❌ Don't commit to version control
- ❌ Don't post in public forums
- ✅ Keep it secure and private

### Best Practices
- ✅ Start with small test clips
- ✅ Verify transcription quality
- ✅ Monitor API usage
- ✅ Keep OpenAI credits funded
- ✅ Review captions before delivery

### Limitations
- Requires internet connection
- Requires valid API key
- Requires OpenAI credits
- Processing time varies by file size
- Accuracy depends on audio quality

---

## 🎉 You're Ready!

Your REDitors Voice-to-Text PRO plugin is:
- ✅ Fully installed
- ✅ Properly configured
- ✅ Production-ready
- ✅ Well-documented

**Start transcribing professional captions today!**

---

**REDitors Voice-to-Text PRO v2.0**  
Professional AI-Powered Transcription for Adobe Premiere Pro

*Transform speech into perfect captions, instantly.* 🎬✨

---

## 📋 Quick Reference Card

```
INSTALLATION:
  Windows: Right-click install-windows.bat → Run as Admin
  macOS:   sudo bash install-macos.sh

CONFIGURATION:
  Edit: js/main.js (line 15)
  Add: Your OpenAI API key

USAGE:
  1. Window → Extensions → REDitors
  2. Select clip on timeline
  3. Click "Select Audio/Video Clip"
  4. Click "Start Transcription"
  5. Click "Create Captions"

VIEW CAPTIONS:
  Window → Markers

EXPORT:
  SRT: Saves to Desktop
  WebVTT: Saves to Desktop
  Text: Copies to clipboard

COST:
  ~$0.006 per minute of audio
  Very affordable!

SUPPORT:
  Read: QUICKSTART.md (daily use)
  Read: README.md (all features)
  Check: Activity Log (in plugin)
```

---

**Need help? Check the other documentation files!**
