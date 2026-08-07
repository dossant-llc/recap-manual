### Problem: Low Volume or Faint Audio

**Symptom:** Recording is very quiet, have to turn volume way up to hear

> ⚠️ **This is about your recording.** If your *callers* say you sound faint, quiet, or distant during the call, that's a different signal path and none of the gain settings below will fix it — see [Callers Say I Sound Muffled or Distant](far-end-audio.md).

**Solutions (try in order):**

**1. ⭐ MOST COMMON: Audio input gain too low**

This fixes 90% of low volume issues!

- **Windows:**
  1. Right-click speaker icon in taskbar
  2. Select "Recording devices"
  3. Double-click "Microphone"
  4. Go to "Levels" tab
  5. Set "Microphone" slider to **100%**
  6. If there's "Microphone Boost" option, try +20dB

- **Mac:**
  1. System Preferences → Sound
  2. Click "Input" tab
  3. Drag "Input volume" slider all the way to the right

**2. Headset microphone position**

- Boom mic should be 1-2 inches from corner of mouth
- Not directly in front (causes breath noise)

**3. Recording software input level**

- Many programs have their own gain slider
- In Audacity: Input level slider at top (set to 0.8-1.0)

**4. Phone call volume**

- During test call, increase phone volume with buttons
- Affects how loud other person sounds in recording

**5. Weak headset microphone**

- Some cheap headsets have poor quality
- Try different headset (Apple EarPods are good reference)

---

### Problem: Audio Routes to Speaker or One Ear with Lightning/USB-C Adapter

**Symptom:** Audio plays through phone speaker instead of headset, or only one ear works — but only when using a Lightning or USB-C to 3.5mm adapter.

**Cause:** When you plug a Lightning or USB-C adapter into your phone, the phone immediately performs accessory detection. It decides whether the accessory is "Headphones," "Headset," or something else (like "Dock speaker"). If the adapter is plugged in without a headset already connected through RECAP, the phone may lock into the wrong audio routing mode.

This affects **all modern phones**:
- **iPhone (Lightning):** Decides "Headphones" vs "Dock speaker" at plug-in
- **iPhone 15+ (USB-C):** Same detection behavior
- **Android (USB-C):** Per the Android spec, USB-C audio adapters don't present audio endpoints until a device is detected and its impedance is measured

**Solution — connect in the right order:**

1. Plug your headset into RECAP's headset jack
2. Plug the recording cable into RECAP's MIC jack (if using a computer)
3. Plug RECAP into the Lightning/USB-C adapter
4. **Plug the adapter into your phone LAST**

**The full chain must be connected before the phone sees it.**

**If you already plugged in wrong order:**

1. Unplug the adapter from the phone
2. Make sure headset is connected to RECAP
3. Plug the adapter back in

**iPhone reset (if it's still routing wrong):**
Settings → Sounds & Haptics → Headphone Safety → USB Accessories → "Forget All" — then reconnect.

**If the order is right and it still misbehaves, check the adapter itself.** Many inexpensive adapters don't carry the microphone channel at all, which leaves your phone using its own built-in microphone — a common reason callers say you sound distant. Tested adapters: <https://recapmycalls.com/compatible-adapters-for-recap/>

**References:**

- [Apple Support — Use Apple wired headphones](https://support.apple.com/en-us/108042)
- [Android AOSP — USB-C audio adapter spec](https://source.android.com/docs/core/interaction/accessories/headset/usb-adapter)

---

### Problem: Can't Hear Call in Headset

**Symptom:** No audio in headset during call (but RECAP is connected)

**Diagnostic:**

1. **Test headset directly with phone (no RECAP)**
   - Does it work?
   - NO → Headset is incompatible, get different one
   - YES → Continue to #2

2. **Check connections**
   - RECAP firmly plugged into phone?
   - Headset firmly plugged into RECAP?
   - Try unplugging and reconnecting firmly

3. **Try different headset**
   - Confirms if it's headset compatibility issue

4. **If none of above work**
   - May be RECAP hardware defect
   - [Contact support](../support.md) with test results

---

### Problem: Static, Noise, or Interference

**Common causes and solutions:**

1. **Loose connections**
   - Ensure all plugs fully inserted
   - Try unplugging and reconnecting firmly

2. **Dirty or damaged connectors**
   - Use compressed air to clean jacks
   - Look for bent pins

3. **Electrical interference**
   - Move RECAP away from power adapters, monitors
   - Don't let cables run parallel to power cords

4. **Microphone gain too high (causing distortion)**
   - Lower gain to 70-80%
   - Look for clipping in waveform (flattened peaks)

5. **Poor quality headset**
   - Some cheap headsets have noisy electronics
   - Try different headset

---

### Problem: Left and Right Channels Are Swapped

**Symptom:** Your voice is on the right channel and the caller is on the left (or vice versa from what you expected)

**This is normal — not a defect.** RECAP's hardware outputs your voice on one channel and the caller's voice on the other, but which is "left" and which is "right" depends on your recording device. USB audio adapters, voice recorders, and some computer sound cards interpret the Tip and Ring pins differently, which can swap the channels.

**How to verify:**

1. Record a short test call
2. Open the recording in Audacity
3. Split Stereo to Mono (track dropdown → Split Stereo to Mono)
4. Play each track — note which is you and which is the caller
5. Label them for future reference

**This only matters if you need to edit channels independently.** If you just play back the full recording, you'll hear both voices regardless of which channel they're on.

**If you need to swap channels in Audacity:**

1. Split Stereo to Mono
2. Drag one track above/below the other to reorder
3. Track dropdown → Make Stereo Track

---

### Problem: Not Working on Mac

**Most Macs have MONO-only or LINE IN ports**

**Diagnostic:**

1. Run device scanner: <https://recapmycalls.com/audio/>
2. Most Macs show MONO only → USB adapter needed

**Mac audio port types:**

- **Combo port** (one port for headphones + mic): Usually MONO only
- **Separate input jack**: Often LINE IN, not MIC IN (incompatible)

**Solution:** Andrea USB stereo adapter - [details here](device-scanner.md)

---

