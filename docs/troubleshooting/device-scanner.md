## The 5-Minute Diagnostic

**Use this flowchart to diagnose ANY problem with RECAP.**

Run tests IN ORDER. Don't skip steps.

### Diagnostic Flowchart

```mermaid
flowchart TD
    Start([Having problems with RECAP?<br/>Start here]) --> Test1{Test 1: Direct Headset Test<br/><br/>Plug headset into phone<br/>Make test call<br/><br/>Can you hear them?<br/>Can they hear you?}

    Test1 -->|NO to either| BadHeadset[❌ STOP<br/><br/>Get different headset<br/>Old headsets from drawers<br/>often don't work<br/><br/>RECAP can't fix<br/>incompatible headsets]

    Test1 -->|YES to both| Test2{Test 2: Pass-Through Test<br/><br/>Connect Phone → RECAP → Headset<br/>Make test call<br/><br/>Can you hear call<br/>in your headset?}

    Test2 -->|NO| TryHeadset[Try different headset<br/>or contact support<br/><br/>May be RECAP defect]

    Test2 -->|YES| Test3{Test 3: Device Scanner<br/><br/>Visit: audio.recapmycalls.com<br/>Take screenshot<br/><br/>STEREO or MONO input?}

    Test3 -->|MONO| USBAdapter[✅ USB Adapter Needed<br/><br/>Andrea USB adapter $20-40<br/><br/>This is NOT a defect<br/>Most modern computers<br/>have MONO inputs<br/><br/>Get adapter, then continue]

    Test3 -->|STEREO| Test4{Test 4: Audio Input Gain<br/><br/>Windows: Recording devices<br/>→ Microphone → Properties<br/>→ Levels → Set to 100%<br/><br/>Mac: System Preferences<br/>→ Sound → Input<br/>→ Drag slider right<br/><br/>Level meter moving?}

    Test4 -->|NO movement| FixGain[✅ Increase gain to 100%<br/><br/>This fixes most<br/>low volume issues!<br/><br/>Also check: correct<br/>input device selected?]

    Test4 -->|YES| Test5{Test 5: Recording Software<br/><br/>Correct mic selected?<br/>STEREO mode enabled?<br/><br/>Make test recording<br/>Play it back}

    Test5 -->|Problems| FixSoftware[✅ Check settings:<br/><br/>- Select External Mic/RECAP<br/>- Enable STEREO recording<br/>- Close apps using mic]

    Test5 -->|Works| Success[✅ Success!<br/><br/>RECAP is working<br/>You're ready to record]

    FixGain --> Retest1[Retest recording]
    FixSoftware --> Retest1
    USBAdapter --> Test4
    Retest1 --> StillBroken{Still not working?}
    StillBroken -->|YES| ContactSupport[📧 Contact Support<br/><br/>Include results from<br/>all 5 tests above]
    StillBroken -->|NO| Success

    style BadHeadset fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style TryHeadset fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style USBAdapter fill:#ffd43b,stroke:#f08c00,color:#000
    style FixGain fill:#ffd43b,stroke:#f08c00,color:#000
    style FixSoftware fill:#ffd43b,stroke:#f08c00,color:#000
    style Success fill:#51cf66,stroke:#2f9e44,color:#fff
    style ContactSupport fill:#748ffc,stroke:#4c6ef5,color:#fff
    style Start fill:#e7f5ff,stroke:#339af0,color:#000
```

**How to use this flowchart:**

1. Start at the top
2. Follow each test in order
3. Yellow boxes = Action needed (fix something)
4. Green box = Success!
5. Red boxes = Stop and get different equipment

---

## The USB Adapter Solution

### When You Need It

**You need a USB stereo adapter if:**

- Device scanner shows "MONO input detected"
- Your computer has no MIC IN port (only LINE IN or combo port)
- Pass-through test works but recording fails
- You have a modern laptop or Mac (most made after 2015 are MONO-only)

### Why This Happens

**RECAP outputs stereo audio (2 channels):**

- One channel = Your voice
- Other channel = Their voice
- ⚠️ Channel assignment (L/R) may vary depending on USB adapter

**Your computer needs stereo input to record both channels.**

Most modern computers save cost by including only MONO microphone inputs. This captures only ONE channel (one-sided audio or no audio).

**This is NOT a RECAP defect** - it's a common computer compatibility issue.

### Recommended Solution: Andrea USB Adapter

**Product:** Andrea USB-SA Audio Adapter
- **Cost:** $20-40 USD
- **Where to buy:** Amazon, B&H Photo, electronics retailers
- **Search for:** "Andrea USB stereo microphone adapter"

**Why we recommend this specific adapter:**

- ✅ Guaranteed stereo microphone input (2 channels)
- ✅ Plug-and-play (no drivers needed)
- ✅ Works on Windows, Mac, Linux
- ✅ Provides proper bias voltage for RECAP
- ✅ Tested and confirmed compatible

### How to Use USB Adapter

**Connections:**

```mermaid
flowchart LR
    Phone[📱 Phone] --> RECAP[⚡ RECAP]
    RECAP --> Headset[🎧 Headset]
    RECAP -->|3.5mm cable| USBAdapter[🔌 USB Adapter<br/>MIC IN jack]
    USBAdapter -->|USB cable| Computer[💻 Computer<br/>USB port]

    style USBAdapter fill:#ffd43b,stroke:#f08c00
```

**Setup steps:**

1. Plug USB adapter into computer's USB port
2. Connect RECAP's output to USB adapter's MIC IN jack
3. Computer will automatically recognize "USB Audio Device"
4. In recording software, select "USB Audio Device" as input
5. Test recording - should now capture both channels

**That's it!** The USB adapter gives your computer a true stereo microphone input.

### Alternative USB Adapters

If Andrea adapter unavailable, look for:

**Required features:**

- **Stereo microphone input** (2 channels) - most important
- Bias voltage for external microphones
- Specifications mention "stereo mic input" or "2-channel input"

**NOT compatible:**

- USB adapters with only LINE IN
- USB adapters with only MONO mic input (1 channel)
- Bluetooth adapters (too much latency for real-time)

---

