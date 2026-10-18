## Frequently Asked Questions

### General Questions

**Q: What is RECAP?**
A: RECAP is a hardware adapter that records both sides of a conversation by splitting headset audio into a stereo signal — your voice on one channel, theirs on the other.

**Q: Do I need special software?**
A: Use recording software that selects the connected external input and captures both stereo channels separately. Verify the result with the [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test).

**Q: What devices work as the CALL source?**
A: A device with an AHJ/CTIA 3.5mm TRRS headset path is a candidate. A working headset establishes a direct-call baseline, not compatibility of the complete RECAP recording chain. Check the [compatibility checklist](getting-started/requirements.md#compatibility-checklist), including microphone-capable adapters/app routing, then run the [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test).

**Q: Can I use RECAP with my computer's headset port?**
A: Yes, as the **call device**. If your computer has a combo headset jack (common on laptops), RECAP plugs into it and you take Zoom, Teams or other calls through your headset. The recording itself goes to a **separate recording device** whose input is a stereo microphone input with plug-in power. See the Zoom question below.

**Q: Do I need batteries?**
A: No batteries are required. Use the supported external stereo MIC-mode setup with plug-in power where supported. Earlier explanations that recorder bias powers S2 were not adequately supported; see the [correction and pending validation](getting-started/requirements.md#plug-in-power-and-voltage-validation-pending).

---

### Compatibility Questions

**Q: Why do I only hear one side of the conversation?**
A: First distinguish one ear in the live headset from a missing recorded channel. A mono recording input is one possibility; wrong input selection, headset/app routing, cabling, gain or processing can also lose a voice. Use [recording troubleshooting](troubleshooting/no-audio.md#problem-recording-only-has-audio-on-one-side) and the [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test); a scanner result alone does not identify the cause.

**Q: Why doesn't RECAP work with my Mac?**
A: Check the actual selected external input against the [compatibility checklist](getting-started/requirements.md#compatibility-checklist). A Mac model name or failed recording does not establish input capability or the cause. If the input is confirmed to lack stereo MIC capture, use a suitable interface; see the [adapter guide](https://recapmycalls.com/compatible-adapters-for-recap/).

**Q: Can I record to my iPhone or Android phone?**
A: Not directly — mobile devices have combo ports, not stereo MIC IN. However, you can use a USB audio adapter (with stereo mic input) connected to your phone's USB-C or Lightning port. This adds a proper stereo input for RECAP. A plain Lightning or USB-C to 3.5mm *headphone* adapter is not enough here. That adapter is the fix for the phone you make calls **on**, not for the one you record **onto**.

**Q: Will RECAP work with my computer?**
A: The [scanner](https://recapmycalls.com/audio/) reports the selected capture path's channel capability. STEREO does not prove the complete chain works, and MONO calls for checking the selected input/mode before choosing an interface. Follow the [compatibility checklist](getting-started/requirements.md#compatibility-checklist) and [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test).

**Q: What's the difference between MIC IN and LINE IN?**
A: Use an external stereo microphone input with MIC mode and plug-in power where supported. Line-only operation is outside the supported setup; port color alone does not establish input capability. See [recorder requirements](getting-started/requirements.md#recording-device-compatibility).

---

### Setup Questions

**Q: Can I hear the call while recording?**
A: Yes! Connect your headset to RECAP and you'll hear the call in real-time while it records.

**Q: Which headset should I use?**
A: A **wired headset with the microphone on the cable**, which means a 4-pole (TRRS) plug with a boom or an inline mic. It also has to work with your phone: plug it straight into the phone and make a call. Apple 3.5mm EarPods work well as a reference. A headset that works with your phone but has **no mic on the cable** will not record your voice, because your phone uses its own built-in microphone instead. See [Headset Compatibility](getting-started/requirements.md#headset-compatibility).

**Q: Why is my recording very quiet?**
A: Check the selected external input, recording gain and processing. Raise gain while watching for clipping, then check each participant's recorded channel in the [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test). Low level alone does not establish a cause.

---

### Recording Questions

**Q: Can I record to a voice recorder instead of computer?**
A: A recorder is a candidate if its external input meets the [recorder checklist](getting-started/requirements.md#recording-device-compatibility). Use stereo MIC mode, plug-in power where supported, and processing off for the initial [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test). Matching specifications are not a physically tested configuration; electrical validation remains pending. Never connect phantom power.

**Q: Can I use RECAP with Zoom, Teams, or Skype calls on my computer?**
A: A computer can be CALL when its AHJ/CTIA wired headset path carries both app audio and the headset mic. Use a separate REC device meeting the [checklist](getting-started/requirements.md#compatibility-checklist), and confirm routing/capture with the [two-sided test](using-recap/making-calls.md#setup-and-two-sided-test). The app name or headset jack alone does not certify the complete chain.

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
A: Never use RECAP with +48V phantom power - it is outside the supported setup. For professional equipment, you may need a different interface.

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

