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

