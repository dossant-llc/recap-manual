### Problem: No Audio Recorded

**Symptom:** Recording file is silent or shows flat waveform

**Run the diagnostic flowchart above. Most common causes:**

1. **Computer has MONO input (most common)**
   - Run scanner: <https://recapmycalls.com/audio/>
   - Solution: USB adapter needed - [details here](device-scanner.md)

2. **Audio input gain too low/muted**
   - Windows: Right-click speaker icon → Recording devices → Microphone → Properties → Levels → Set to **100%**
   - Mac: System Preferences → Sound → Input → Drag slider all the way right
   - Speak into headset - do you see level meter moving?

3. **Headset incompatible with phone**
   - Test headset directly with phone (no RECAP)
   - Old headsets from drawers often don't work

4. **Connected to LINE IN instead of MIC IN**
   - LINE IN has no bias voltage, won't power RECAP
   - Look for port with microphone icon or pink color

5. **Wrong input device selected in software**
   - Check recording software settings
   - Select "RECAP" or "External Microphone"

---

### Problem: Only Hear in One Ear (Headset)

**Symptom:** During a call with RECAP connected, you only hear the caller in one ear of your headset.

**This is NOT the stereo split.** The stereo split only applies to the recording output (the cable going to your computer). The headset pass-through is transparent — it forwards your phone's audio to your headset untouched, exactly like plugging the headset directly into your phone. You should hear in both ears. See [How RECAP Works](../using-recap/making-calls.md) for details.

**If you only hear in one ear, check these:**

1. **Headset plugged into wrong jack**
   - RECAP has two output jacks: the headset pass-through and the MIC recording output
   - If your headset is in the MIC jack, you'll hear the stereo split (one side per ear) instead of normal call audio
   - Move the headset to the pass-through jack

2. **Cable not fully seated**
   - Push the headset plug firmly into RECAP until it clicks
   - Do the same for the phone-to-RECAP connection
   - A partial insert can drop a channel

3. **Headset problem**
   - Test the headset directly in your phone (no RECAP)
   - If it's still one ear, the headset is the issue

4. **Phone adapter issue**
   - If using a Lightning or USB-C to 3.5mm adapter, try a different one
   - Some cheap adapters don't pass all channels correctly

---

### Problem: Recording Only Has Audio on One Side

**Symptom:** You open your recording and only one channel has audio — the other is silent or very quiet.

**This IS about the recording output** (not the headset). Most common cause:

1. **Computer has MONO input (most common)**
   - Most modern laptops and all Macs have mono-only mic inputs
   - A mono input can only capture one of RECAP's two channels
   - Run the [Audio Device Scanner](https://recapmycalls.com/audio/) to check
   - Solution: USB stereo audio adapter — [details here](device-scanner.md)

2. **Echo cancellation or noise suppression enabled**
   - These features can merge or suppress one channel
   - Run the scanner, expand your device, and disable Echo Cancellation and Noise Suppression
   - See [Device Scanner guide](device-scanner.md) for details

3. **USB adapter swapping channels**
   - Some USB adapters reverse left and right
   - Not a problem — just note which channel is you and which is the caller

---

