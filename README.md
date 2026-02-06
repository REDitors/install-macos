# 🎬 REDitors Voice-to-Text PRO v2.0

## Professional AI-Powered Transcription & Captioning for Adobe Premiere Pro

Transform your video editing workflow with cutting-edge AI transcription technology. REDitors Voice-to-Text PRO brings professional-grade speech recognition directly into Premiere Pro with an intuitive, powerful interface.

---

## 🌟 What's New in v2.0

### ✨ Major Enhancements

- **🎨 Modern UI Redesign** - Sleek, professional interface with gradient designs and smooth animations
- **⚡ Advanced AI Models** - Support for Whisper Large, Medium, and v1 models
- **👥 Speaker Diarization** - Automatically identify different speakers in your audio
- **🌐 Auto Language Detection** - Let AI detect the language automatically
- **✂️ Smart Caption Splitting** - Automatically split long captions (42 char limit)
- **📊 Real-time Statistics** - View word count, segment count, and duration
- **🎯 Confidence Filtering** - Filter out low-confidence transcriptions
- **📝 Smart Punctuation** - Enhanced punctuation for better readability
- **🚫 Profanity Filter** - Optional content filtering
- **📄 WebVTT Export** - Export to web video text track format
- **📋 Quick Copy** - Copy full transcription to clipboard
- **🎨 Tabbed Settings** - Basic and Advanced settings organization
- **⏱️ Processing Timer** - Track how long transcription takes
- **🔍 Enhanced Logging** - Color-coded activity log with icons
- **💾 Better File Handling** - Improved error handling and validation

### 🎯 Enhanced Features

- Multi-model support (Whisper v1, Medium, Large)
- Advanced transcription options
- Improved caption creation
- Multiple export formats (SRT, WebVTT)
- Better error messages and debugging
- Smoother progress tracking
- Professional statistics display
- Quick action shortcuts
- Enhanced marker creation with colors

---

## 🚀 Quick Start

### Installation

#### Windows
```bash
# Run as Administrator
install-windows.bat
```

#### macOS
```bash
sudo bash install-macos.sh
```

### Configuration

1. Open `js/main.js`
2. Line 15: Replace with your OpenAI API key:
```javascript
const API_KEY = 'your-openai-api-key-here';
```

3. Restart Premiere Pro
4. Go to `Window` → `Extensions` → `REDitors Voice-to-Text PRO`

---

## 📖 Complete Features List

### 🎙️ Transcription Features

- ✅ **13+ Languages** - English, Spanish, French, German, Italian, Portuguese, Arabic, Chinese, Japanese, Korean, Russian, Hindi, Turkish
- ✅ **Multiple AI Models** - Choose between Whisper v1 (fast), Medium (balanced), or Large (most accurate)
- ✅ **Auto Language Detection** - Let AI identify the language
- ✅ **Speaker Diarization** - Identify different speakers (when enabled)
- ✅ **Smart Punctuation** - AI-enhanced punctuation and formatting
- ✅ **Confidence Filtering** - Filter words below your confidence threshold
- ✅ **Profanity Filter** - Optional content filtering

### 💬 Caption Features

- ✅ **Automatic Markers** - Creates sequence markers with captions
- ✅ **Smart Splitting** - Splits captions longer than 42 characters
- ✅ **Auto-sync** - Syncs captions to clip timecode
- ✅ **Color-coded Markers** - Blue markers for easy identification
- ✅ **Speaker Labels** - Adds speaker names to captions (when detected)
- ✅ **Full Text in Comments** - Complete caption text in marker comments

### 📤 Export Features

- ✅ **SRT Export** - Standard subtitle format with UTF-8 BOM
- ✅ **WebVTT Export** - Modern web video text track format
- ✅ **Clipboard Copy** - Quick copy of full transcription
- ✅ **Automatic Naming** - Smart file naming with date stamps
- ✅ **Desktop Save** - Quick access to exported files

### 📊 Analysis Features

- ✅ **Word Count** - Total words in transcription
- ✅ **Segment Count** - Number of caption segments
- ✅ **Duration Display** - Total audio duration
- ✅ **Processing Time** - Track transcription speed
- ✅ **File Size Info** - Display media file size

### 🎨 Interface Features

- ✅ **Modern Design** - Professional gradient UI with smooth animations
- ✅ **Tabbed Settings** - Basic and Advanced settings organization
- ✅ **Quick Actions** - One-click export and copy functions
- ✅ **Real-time Progress** - Detailed progress bar with labels
- ✅ **Status Indicators** - Clear success/error/processing states
- ✅ **Activity Log** - Color-coded log with timestamps
- ✅ **Responsive Layout** - Adapts to panel size

---

## 🎯 How to Use

### Basic Workflow

1. **Select Clip**
   - Select a video/audio clip on timeline
   - Click "📌 Select Audio/Video Clip"
   - Verify clip info appears

2. **Configure Settings**
   - Choose language (or enable auto-detect)
   - Select AI model (Whisper v1 recommended)
   - Optional: Configure advanced settings

3. **Transcribe**
   - Click "🎙️ Start Transcription"
   - Wait for AI processing (10-30 seconds per minute of audio)
   - View statistics when complete

4. **Create Captions**
   - Choose caption track (new or existing)
   - Enable auto-sync for timecode alignment
   - Click "✨ Create Captions"
   - Captions appear as sequence markers

5. **Export** (Optional)
   - Click "📄 Export SRT File" for subtitle file
   - Click "🌐 Export WebVTT" for web format
   - Click "📋 Copy Full Text" for clipboard

### Advanced Settings

#### Auto Language Detection
Enable to let AI detect the language automatically. Works great for multilingual content!

#### Speaker Diarization
Identifies different speakers in your audio. Speakers labeled as [Speaker 1], [Speaker 2], etc.

#### Smart Punctuation
AI adds proper punctuation, capitalization, and formatting to make captions more readable.

#### Profanity Filter
Filters inappropriate language from transcriptions.

#### Confidence Threshold
Filter out words below a certain confidence level (0-100%). Higher = stricter filtering.

#### Split Long Captions
Automatically splits captions longer than 42 characters for better readability on screen.

---

## 🎨 UI Guide

### Header
- **Version Badge** - Shows current version (v2.0 PRO)
- **Title** - Plugin name with emoji
- **Subtitle** - Quick description

### Clip Selection Panel
- **Select Button** - Choose timeline clip
- **Info Box** - Shows sequence, clip name, duration

### Transcription Settings Panel
- **Basic Tab** - Language and model selection
- **Advanced Tab** - Fine-tuning options and filters
- **Settings Controls** - Checkboxes and sliders

### Processing Panel
- **Transcribe Button** - Start AI processing
- **Progress Bar** - Real-time progress with labels
- **Status Display** - Current operation status
- **Statistics Grid** - Words, segments, duration

### Caption Creation Panel
- **Track Selector** - Choose caption track
- **Options** - Auto-sync and split settings
- **Create Button** - Generate captions
- **Quick Actions** - Export and copy shortcuts

### Activity Log Panel
- **Log Display** - Color-coded activity feed
- **Clear Button** - Reset log
- **Timestamps** - All actions timestamped
- **Icons** - Visual status indicators

---

## 🔧 Advanced Usage

### Working with Multiple Clips

Process each clip separately:
1. Select clip 1, transcribe, create captions
2. Select clip 2, transcribe, create captions
3. All captions accumulate in sequence

### Multi-Language Projects

For videos with multiple languages:
1. Transcribe each language section separately
2. Change language setting for each
3. Create separate caption tracks
4. Or use different marker colors

### Batch Processing Tips

1. **Organize Clips** - Group by language/speaker
2. **Process in Order** - Start from beginning of timeline
3. **Export Separately** - Export SRT for each clip
4. **Merge Files** - Combine SRT files if needed

### Quality Optimization

**For Best Accuracy:**
- Use high-quality audio
- Clean audio in Audition first
- Normalize audio levels
- Remove background noise
- Use Whisper Large model
- Enable smart punctuation

**For Speed:**
- Use Whisper v1 model
- Shorter clips process faster
- Disable speaker diarization
- Lower confidence threshold

---

## 📊 Supported Formats

### Input Audio Formats
- ✅ MP3, MP4, M4A
- ✅ WAV, AIFF, AIF
- ✅ MXF, MOV, AVI
- ✅ MKV, WebM
- ✅ FLAC, OGG
- ✅ Any format Premiere Pro imports

### Output Formats
- ✅ **Sequence Markers** - Native Premiere Pro
- ✅ **SRT** - Universal subtitle format
- ✅ **WebVTT** - Modern web format
- ✅ **Plain Text** - Via clipboard

### File Size Limits
- **Recommended:** Under 25MB
- **Maximum:** Depends on API provider
- **Large Files:** May take longer to process

---

## 🎓 Tips & Tricks

### Pro Tips

**1. Prepare Audio First**
- Clean audio = better transcription
- Use Premiere's audio effects
- Or edit in Audition first

**2. Use Markers Effectively**
- Markers show in Markers panel
- Double-click to jump to caption
- Edit marker text to fix typos
- Color-code different speakers

**3. Export Strategy**
- Use markers for reference
- Export SRT for final captions
- Import SRT to caption track
- Full editing in caption track

**4. Keyboard Shortcuts**
- `M` - Add/edit marker
- `Window` → `Markers` - View all
- `Shift+M` - Next marker
- `Ctrl+Shift+M` - Previous marker

**5. Quality Check**
- Review transcription before creating captions
- Check activity log for errors
- Use confidence filtering
- Proofread exported files

### Common Workflows

**Social Media Captions:**
```
1. Transcribe with auto-sync
2. Enable caption splitting (42 chars)
3. Create captions as markers
4. Export SRT
5. Import to caption track
6. Style and burn into video
```

**YouTube Closed Captions:**
```
1. Transcribe full video
2. Export SRT file
3. Upload video + SRT to YouTube
4. YouTube displays as CC
```

**Professional Broadcast:**
```
1. Use Whisper Large model
2. Enable smart punctuation
3. Speaker diarization ON
4. Create captions
5. Export to professional format
6. Review and edit in caption track
```

**Multi-Language Content:**
```
1. Split clips by language
2. Transcribe each separately
3. Change language setting
4. Create separate tracks
5. Export individual SRT files
```

---

## 🐛 Troubleshooting

### Plugin Not Showing

**Issue:** Extension doesn't appear in Window menu

**Solutions:**
- Restart Premiere Pro completely
- Check installation path is correct
- Enable CEP debug mode (installer does this)
- Check if extension folder has all files

### API Errors

**Issue:** "API Error 401" or "API Error 429"

**Solutions:**
- Check API key is correct
- Verify internet connection
- Check API quota/limits
- Wait and try again (rate limit)

### File Path Errors

**Issue:** "Could not get media file path"

**Solutions:**
- Clip must be imported media, not:
  - Nested sequences
  - Titles or graphics
  - Adjustment layers
  - Generated content
- Relink offline media
- Ensure file hasn't been moved

### No Captions Created

**Issue:** Transcription works but no markers

**Solutions:**
- Check sequence is active
- Review activity log for errors
- Try creating new sequence
- Check Premiere Pro version compatibility
- Look in Markers panel (`Window` → `Markers`)

### Poor Accuracy

**Issue:** Transcription has many errors

**Solutions:**
- Use Whisper Large model
- Clean audio first
- Specify correct language
- Check audio quality
- Increase confidence threshold

### Processing Timeout

**Issue:** "Request timed out"

**Solutions:**
- File may be too large (>25MB)
- Split into smaller clips
- Check internet speed
- Try again later
- Use shorter clips

---

## 🔌 System Requirements

### Software
- **Adobe Premiere Pro** 2020 or later (CC 2020-2024)
- **Operating System** Windows 10+ or macOS 10.14+
- **Internet** Required for API calls

### Hardware
- **RAM** 8GB minimum, 16GB recommended
- **Storage** 100MB for plugin
- **Network** Stable connection required

### API Requirements
- OpenAI API key (or compatible provider)
- Active API subscription
- Sufficient API credits/quota

---

## 🆚 Comparison: v1.0 vs v2.0

| Feature | v1.0 | v2.0 PRO |
|---------|------|----------|
| UI Design | Basic B&W | Modern Gradient |
| AI Models | Whisper v1 only | v1, Medium, Large |
| Languages | 10 | 13+ |
| Speaker ID | ❌ | ✅ |
| Auto Language | ❌ | ✅ |
| Caption Splitting | ❌ | ✅ |
| Statistics | ❌ | ✅ |
| WebVTT Export | ❌ | ✅ |
| Quick Copy | ❌ | ✅ |
| Advanced Settings | ❌ | ✅ |
| Confidence Filter | ❌ | ✅ |
| Progress Labels | Basic | Detailed |
| Error Messages | Generic | Specific |
| Processing Timer | ❌ | ✅ |
| Color-coded Log | ❌ | ✅ |
| Tab Interface | ❌ | ✅ |

---

## 📝 API Configuration Guide

### OpenAI Whisper API (Recommended)

1. **Get API Key**
   - Go to https://platform.openai.com
   - Sign up or log in
   - Navigate to API Keys
   - Create new secret key

2. **Configure Plugin**
   ```javascript
   const API_KEY = 'sk-...your-key-here...';
   const API_ENDPOINT = 'https://api.openai.com/v1/audio/transcriptions';
   ```

3. **Pricing**
   - $0.006 per minute
   - Very affordable for professional use

### Alternative Providers

The plugin can work with any Whisper-compatible API:

**AssemblyAI:**
```javascript
const API_KEY = 'your-assemblyai-key';
const API_ENDPOINT = 'https://api.assemblyai.com/v2/transcript';
```

**Deepgram:**
```javascript
const API_KEY = 'your-deepgram-key';
const API_ENDPOINT = 'https://api.deepgram.com/v1/listen';
```

**Custom API:**
Any API that accepts audio files and returns JSON with segments.

---

## 🎯 Best Practices

### Before Transcribing

- ✅ Review and clean audio
- ✅ Normalize levels
- ✅ Remove long silences
- ✅ Check file is properly linked
- ✅ Verify internet connection

### During Transcription

- ✅ Monitor progress bar
- ✅ Check activity log
- ✅ Don't close Premiere Pro
- ✅ Wait for completion
- ✅ Review statistics

### After Transcription

- ✅ Check word count makes sense
- ✅ Review a few random segments
- ✅ Create captions
- ✅ Export for backup
- ✅ Proofread before delivery

### Quality Assurance

1. **Accuracy Check** - Review random samples
2. **Timing Check** - Verify sync is correct
3. **Format Check** - Ensure proper capitalization
4. **Completeness Check** - All dialogue captured
5. **Export Verification** - Open exported file

---

## 🔐 Security & Privacy

### Data Handling

- Audio sent to API for processing
- Transcriptions stored locally only
- No data permanently stored by plugin
- API provider privacy policy applies

### Best Practices

- Use secure API keys
- Don't share API keys
- Rotate keys periodically
- Review API usage regularly
- Check provider's data policies

---

## 📚 Additional Resources

### Documentation
- `README.md` - This file (comprehensive guide)
- `QUICKSTART.md` - Quick reference guide
- `BUGFIX.md` - Bug fix history and solutions

### Support
- Check activity log for detailed errors
- Review troubleshooting section
- Consult Premiere Pro documentation
- Check API provider status

### Community
- Share your workflows
- Report issues
- Suggest features
- Help other users

---

## 🎬 Example Workflows

### YouTube Video
1. Edit video completely
2. Select audio track
3. Transcribe with English (or auto-detect)
4. Create captions with auto-sync
5. Export SRT file
6. Upload video + SRT to YouTube

### Corporate Training
1. Record training video
2. Clean audio in Audition
3. Transcribe with speaker diarization
4. Create captions
5. Export to professional format
6. Review and edit for accuracy

### Documentary
1. Interview clips
2. Transcribe each separately
3. Use speaker diarization
4. Create markers for reference
5. Export SRT for each section
6. Combine and edit

### Social Media
1. Short-form content
2. Quick transcription
3. Enable caption splitting
4. Burn captions into video
5. Export for Instagram/TikTok

---

## 🚀 Future Enhancements

### Planned Features
- [ ] Real-time transcription during recording
- [ ] Custom vocabulary support
- [ ] Translation to multiple languages
- [ ] Batch processing multiple clips
- [ ] Cloud storage integration
- [ ] Advanced timeline integration
- [ ] Custom caption styles
- [ ] Export to more formats
- [ ] Automatic backup

### Under Consideration
- Timeline markers with thumbnails
- Integration with other Adobe apps
- Local AI model support (offline)
- Custom API endpoints
- Advanced editing features

---

## 📄 License

**REDitors Voice-to-Text PRO**
Professional Edition v2.0

Commercial License
© 2024 REDitors. All Rights Reserved.

This plugin requires:
- Valid Adobe Premiere Pro license
- OpenAI API subscription (or compatible provider)
- Proper attribution when redistributing

---

## 🙏 Credits

**Developed by REDitors**
Professional Video Production Tools

**Powered by:**
- OpenAI Whisper API
- Adobe CEP Framework
- Node.js

**Special Thanks:**
- Adobe Premiere Pro team
- OpenAI team
- Professional editors providing feedback

---

## 📞 Support

For technical support:
1. Check this README thoroughly
2. Review the activity log
3. Consult troubleshooting section
4. Check API provider status
5. Verify configuration

**Remember:** The activity log is your best friend for debugging!

---

## 🎉 Get Started Now!

1. Install the plugin
2. Configure your API key
3. Select a clip
4. Click transcribe
5. Create amazing captions!

**REDitors Voice-to-Text PRO** - Transform speech into perfect captions, instantly.

*Professional tools for professional editors.* 🎬✨