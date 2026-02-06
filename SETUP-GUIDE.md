# 🚀 REDitors Voice-to-Text PRO - Complete Setup Guide

## ✅ Plugin Status: READY TO USE

All files are properly organized and the plugin is fully functional!

---

## 📁 File Structure

```
REDitors-VoiceToText-PremierePro/
├── CSXS/
│   └── manifest.xml          # Plugin configuration
├── js/
│   ├── libs/
│   │   └── CSInterface.js    # Adobe CEP library
│   └── main.js               # Main plugin logic
├── jsx/
│   └── hostscript.jsx        # ExtendScript for Premiere Pro
├── icons/
│   └── icon-info.txt         # Icon placeholder info
├── index.html                # Plugin UI
├── .debug                    # Debug configuration
├── install-windows.bat       # Windows installer
├── install-macos.sh          # macOS installer
├── README.md                 # Full documentation
├── QUICKSTART.md             # Quick start guide
├── BUGFIX.md                 # Bug fix documentation
└── package.json              # Plugin metadata
```

---

## 🔧 Installation Instructions

### Windows

1. **Run Installer as Administrator:**
   ```
   Right-click install-windows.bat → "Run as administrator"
   ```

2. **The installer will:**
   - Create the plugin folder at: `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro`
   - Copy all files
   - Enable CEP debug mode
   - Set proper permissions

3. **Continue to Configuration step below**

### macOS

1. **Run Installer with sudo:**
   ```bash
   sudo bash install-macos.sh
   ```

2. **The installer will:**
   - Create the plugin folder at: `/Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro`
   - Copy all files
   - Enable CEP debug mode
   - Set proper permissions

3. **Continue to Configuration step below**

---

## ⚙️ Configuration (CRITICAL)

### Step 1: Add Your OpenAI API Key

**IMPORTANT:** The plugin will NOT work without a valid API key!

1. **Navigate to the installed plugin folder:**
   - **Windows:** `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro\js\`
   - **macOS:** `/Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro/js/`

2. **Open `main.js` in a text editor** (Notepad++, VS Code, or TextEdit)

3. **Find line 15:**
   ```javascript
   const API_KEY = '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';
   ```

4. **Replace with YOUR OpenAI API key:**
   ```javascript
   const API_KEY = 'sk-YOUR-ACTUAL-API-KEY-HERE';
   ```

5. **Save the file**

### Step 2: Get an OpenAI API Key (if you don't have one)

1. Go to: https://platform.openai.com/api-keys
2. Sign up or log in
3. Click "Create new secret key"
4. Copy the key (starts with `sk-...`)
5. Add credits to your account at https://platform.openai.com/account/billing
6. Use the key in Step 1 above

---

## 🎬 Using the Plugin

### Step 1: Open Plugin in Premiere Pro

1. **Start Adobe Premiere Pro**
2. Go to: **Window → Extensions → REDitors**
3. The plugin panel will open

### Step 2: Transcribe Audio

1. **Select a clip** on your timeline (must be audio/video with audio)
2. Click **"📌 Select Audio/Video Clip"**
3. Choose your **language** from dropdown
4. Click **"🎙️ Start Transcription"**
5. Wait for transcription to complete (10-30 seconds typically)

### Step 3: Create Captions

1. After transcription completes, click **"✨ Create Captions"**
2. Captions will be added as **sequence markers** on your timeline
3. View them in: **Window → Markers**

### Step 4: Export (Optional)

- **SRT File:** Click "📄 Export SRT File" - saves to Desktop
- **WebVTT File:** Click "🌐 Export WebVTT" - saves to Desktop
- **Copy Text:** Click "📋 Copy Full Text" - copies to clipboard

---

## 🎯 Features Overview

### Transcription
- ✅ AI-powered speech recognition (OpenAI Whisper)
- ✅ 13+ languages supported
- ✅ 3 AI models (Whisper v1, Medium, Large)
- ✅ Auto language detection
- ✅ Speaker diarization (identifies different speakers)
- ✅ Smart punctuation
- ✅ Confidence filtering

### Captions
- ✅ Automatic sequence marker creation
- ✅ Smart caption splitting (42 character limit)
- ✅ Auto-sync to clip timecode
- ✅ Color-coded markers
- ✅ Speaker labels

### Export Formats
- ✅ SRT (SubRip)
- ✅ WebVTT (Web Video Text Tracks)
- ✅ Plain text (clipboard)

---

## 🔍 Troubleshooting

### Plugin Not Showing in Premiere Pro?

**Solution 1: Enable CEP Debug Mode Manually**

**Windows:**
1. Press `Win + R`
2. Type `regedit` and press Enter
3. Navigate to: `HKEY_CURRENT_USER\Software\Adobe\CSXS.11`
4. Create/edit `PlayerDebugMode` → Set value to `1`
5. Restart Premiere Pro

**macOS:**
1. Open Terminal
2. Run: `defaults write com.adobe.CSXS.11 PlayerDebugMode 1`
3. Restart Premiere Pro

**Solution 2: Check Installation Path**

Verify files are in the correct location:
- Windows: `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\REDitors-VoiceToText-PremierePro`
- macOS: `/Library/Application Support/Adobe/CEP/extensions/REDitors-VoiceToText-PremierePro`

**Solution 3: Restart Premiere Pro Completely**
- Close ALL Premiere Pro windows
- Wait 10 seconds
- Reopen Premiere Pro

### API Errors?

**"Invalid API Key"**
- Check that you added your API key to line 15 of `js/main.js`
- Make sure the key is in quotes: `'sk-...'`
- Verify the key is valid at https://platform.openai.com/api-keys

**"Insufficient Credits"**
- Add credits to your OpenAI account
- Go to: https://platform.openai.com/account/billing

**"Network Error"**
- Check your internet connection
- Try again in a few moments
- OpenAI API might be temporarily down

### Can't Select Clip?

**Must be:**
- ✅ An imported media file (audio or video)
- ✅ Selected on the timeline
- ✅ In an active sequence

**Cannot be:**
- ❌ Title/graphic
- ❌ Nested sequence
- ❌ Adjustment layer

### No Captions Created?

1. Check **Window → Markers** panel
2. Make sure transcription completed successfully
3. Check the Activity Log in the plugin for errors
4. Try with a shorter clip first (10-20 seconds)

---

## 📊 Supported Languages

🇬🇧 English | 🇪🇸 Spanish | 🇫🇷 French | 🇩🇪 German  
🇮🇹 Italian | 🇵🇹 Portuguese | 🇸🇦 Arabic | 🇨🇳 Chinese  
🇯🇵 Japanese | 🇰🇷 Korean | 🇷🇺 Russian | 🇮🇳 Hindi | 🇹🇷 Turkish

---

## 💡 Pro Tips

### For Best Accuracy
1. Use **Whisper Large** model for professional work
2. Specify the correct **language** (don't rely on auto-detect for critical work)
3. Enable **Smart Punctuation**
4. Use clean, normalized audio

### For Speed
1. Use **Whisper v1** model
2. Process shorter clips (under 5 minutes)
3. Disable speaker diarization if not needed

### For Workflow Efficiency
1. Process clips in order
2. Export SRT files for each section
3. Use markers for quick reference
4. Import SRT to caption track for final editing

---

## 🔄 Version Information

**Current Version:** 2.0.0  
**Plugin Type:** Adobe CEP Extension  
**Compatible With:** Premiere Pro 2020 - 2024  
**Requires:** Internet connection, OpenAI API key

---

## 📚 Additional Documentation

- **README.md** - Comprehensive feature documentation
- **QUICKSTART.md** - Quick reference guide
- **BUGFIX.md** - Bug fix history and solutions

---

## ✅ Pre-Installation Checklist

Before you start:
- [ ] Adobe Premiere Pro installed (2020 or later)
- [ ] Administrator/sudo access
- [ ] OpenAI API account created
- [ ] API key obtained
- [ ] Credits added to OpenAI account
- [ ] Internet connection available

---

## 🚀 Quick Start (60 Seconds)

1. **Install:** Run installer with admin/sudo
2. **Configure:** Add API key to `js/main.js` line 15
3. **Restart:** Restart Premiere Pro
4. **Use:** Window → Extensions → REDitors
5. **Transcribe:** Select clip → Transcribe → Create Captions

---

## 🎉 You're Ready!

The plugin is fully configured and ready to use. Start transcribing!

**Questions?** Check the comprehensive README.md file.

**REDitors Voice-to-Text PRO** - Professional AI transcription for professional editors.
