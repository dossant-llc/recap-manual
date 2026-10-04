## Frequently Asked Questions

### General Questions

**Q: What is RECAP?**
A: RECAP is a hardware adapter that records both sides of a conversation by splitting headset audio into a stereo signal — your voice on one channel, theirs on the other.

**Q: Do I need special software?**
A: No. Any recording software works (Windows Sound Recorder, Mac QuickTime, Audacity, etc.). We recommend Audacity (free) for best features.

**Q: What devices work as the CALL source?**
A: Any device with a 3.5mm combo headset port (TRRS) — phones, tablets, laptops, even desktops with combo jacks. If your headset works with it, RECAP will work.

**Q: Can I use RECAP with my computer's headset port?**
A: Yes, as the **call device**. If your computer has a combo headset jack (common on laptops), RECAP plugs into it and you take Zoom, Teams or other calls through your headset. The recording itself goes to a **separate recording device** whose input is a stereo microphone input with plug-in power. See the Zoom question below.

**Q: Do I need batteries?**
A: No. RECAP draws a small plug-in power (bias voltage) from the microphone input of your recording device: a computer mic input, a USB audio adapter, or a voice recorder. That input has to supply it. A LINE IN does not.

---

### Compatibility Questions

**Q: Why do I only hear one side of the conversation?**
A: Your computer has a MONO microphone input (captures only one channel). Run the scanner at <https://recapmycalls.com/audio/> to confirm. Solution: a USB adapter that adds a [stereo mic input](https://recapmycalls.com/compatible-adapters-for-recap/).

**Q: Why doesn't RECAP work with my Mac?**
A: Most modern Macs have MONO inputs or LINE IN ports (not MIC IN). You need a USB adapter that adds a stereo mic input — see the [compatible adapters guide](https://recapmycalls.com/compatible-adapters-for-recap/).

**Q: Can I record to my iPhone or Android phone?**
A: Not directly — mobile devices have combo ports, not stereo MIC IN. However, you can use a USB audio adapter (with stereo mic input) connected to your phone's USB-C or Lightning port. This adds a proper stereo input for RECAP. A plain Lightning or USB-C to 3.5mm *headphone* adapter is not enough here. That adapter is the fix for the phone you make calls **on**, not for the one you record **onto**.

**Q: Will RECAP work with my computer?**
A: Check compatibility with our free scanner: <https://recapmycalls.com/audio/>. If it shows STEREO input, yes. If MONO, you'll need a USB adapter.

**Q: What's the difference between MIC IN and LINE IN?**
A: MIC IN provides bias voltage to power RECAP and has amplification for microphone signals. LINE IN has neither (RECAP won't work). MIC IN is usually pink, LINE IN is usually blue.

---

### Setup Questions

**Q: Can I hear the call while recording?**
A: Yes! Connect your headset to RECAP and you'll hear the call in real-time while it records.

**Q: Which headset should I use?**
A: A **wired headset with the microphone on the cable**, which means a 4-pole (TRRS) plug with a boom or an inline mic. It also has to work with your phone: plug it straight into the phone and make a call. Apple 3.5mm EarPods work well as a reference. A headset that works with your phone but has **no mic on the cable** will not record your voice, because your phone uses its own built-in microphone instead. See [Headset Compatibility](getting-started/requirements.md#headset-compatibility).

**Q: Why is my recording very quiet?**
A: Audio input gain is almost always the issue. Set your computer's microphone gain to 100%. This fixes 90% of low volume issues.

---

### Recording Questions

**Q: Can I record to a voice recorder instead of computer?**
A: Yes, if its external microphone input is **stereo and supplies plug-in power**. Check your recorder's manual. Set it to STEREO (not mono) and to MIC (not line), with any noise reduction or auto level turned off. Never use an input with 48V phantom power.

**Q: Can I use RECAP with Zoom, Teams, or Skype calls on my computer?**
A: Yes, if your computer uses a combo headset port (3.5mm TRRS). Connect: Computer → RECAP → Headset, then record to a second device (voice recorder, another computer, or phone with USB audio adapter). Unlike built-in recording features, RECAP doesn't notify other participants that you're recording.

**Q: What recording quality should I use?**
A: For best quality: WAV format, 44.1kHz or 48kHz sample rate, 16-bit depth. For smaller files: MP3 at 192kbps or higher.

**Q: Can I record on both sides in separate files?**
A: Yes, in Audacity. Record in stereo, then use "Split Stereo Track". Each voice lands on its own track. Which one is left and which is right depends on your recording device, so play each track once and label it (see [Channel Swap](troubleshooting/low-volume-noise.md#problem-left-and-right-channels-are-swapped)).

---

### Troubleshooting Questions

**Q: My headset works with my phone but not with RECAP. Why?**
A: This is rare but can happen with unusual headset wiring. Try a different headset (Apple EarPods are a good test). If multiple headsets fail, contact support.

**Q: I hear static or noise. What's wrong?**
A: Check all connections are firm. Move RECAP away from power adapters. Lower microphone gain to 70-80%. Try a different headset.

**Q: Can I use a splitter cable to record to multiple devices?**
A: No supported configuration for splitters exists.

---

### Product Questions

**Q: Is RECAP wireless/Bluetooth?**
A: No. RECAP is a wired hardware adapter. Bluetooth has too much latency for real-time call recording.

**Q: Can I use RECAP with a mixer or recording equipment?**
A: Never use RECAP with +48V phantom power - it will damage the device. For professional equipment, you may need a different interface.

**Q: How long does RECAP last?**
A: RECAP has no batteries or moving parts. With proper care, it should last indefinitely.

---

### Technical Questions

**Q: What is MONO vs STEREO input?**
A: STEREO input has 2 channels (can record left and right separately). MONO input has 1 channel (records only one side). RECAP requires STEREO to record both sides of conversation.

**Q: What is AHJ standard?**
A: American Headset Jack - the standard headphone connector pinout used by iPhone, Android, and most cell phones. Opposite of OMTP (rare, older phones).

**Q: Why does the scanner show my input as MONO?**
A: Most laptops and Macs made after 2015 have MONO-only inputs to save cost. This is normal. Solution: USB adapter.

---

