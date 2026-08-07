## Quick Start: 4 Steps

### Step 1: Test Your Headset (2 minutes)

**⚠️ DO NOT SKIP THIS STEP**

Many people grab an old headset from a drawer that doesn't work with their phone. Test it FIRST before connecting RECAP.

**How to test:**

1. Plug headset directly into your phone (no RECAP)
2. Make a test call to a friend or voicemail
3. Check:
   - ✅ Can you hear them clearly?
   - ✅ Can they hear you clearly?

**Results:**

- ✅ **Both YES** → Headset works! Continue to Step 2
- ❌ **Either NO** → **STOP.** Get a different headset before continuing

**Why this matters:** If your headset doesn't work with your phone directly, RECAP cannot fix it.

> **"They can hear me, but they say I sound muffled or distant."** That usually means there's no microphone on the headset cable, or the adapter isn't carrying the mic channel — see [Callers Say I Sound Muffled or Distant](../troubleshooting/far-end-audio.md). Sort this out before adding RECAP; RECAP can't improve what the phone is already sending.

---

### Step 2: Pass-Through Test (2 minutes)

**⚠️ You DON'T need your computer for this test**

This verifies RECAP hardware is working before you connect to computer.

**Make the connections:**

```
Phone ──→ RECAP ──→ Headset
```

**Connection details:**

1. Plug your headset into RECAP's headset jack
2. Plug RECAP into your phone's headphone jack (or Lightning/USB-C adapter)
3. **Don't connect to computer yet**

> ⚠️ **Connection order matters.** Always connect the headset to RECAP **before** plugging RECAP into your phone. When a Lightning or USB-C adapter is plugged in, your phone immediately decides how to route audio. If the headset isn't already in the chain, the phone may not recognize it as a headset setup — causing audio to route to the speaker instead. See [Connection Order troubleshooting](../troubleshooting/low-volume-noise.md#problem-audio-routes-to-speaker-or-one-ear-with-lightningusb-c-adapter) for details.

**Pass-through test:**

1. Make a test call on your phone
2. **Can you hear the call clearly in your headset?**

**Results:**

- ✅ **YES** → RECAP hardware works! Continue to Step 3
- ❌ **NO** → Either bad headset (redo Step 1) or hardware issue ([contact support](../support.md))

---

### Step 3: Check Computer Compatibility (1 minute)

**⚠️ BEFORE plugging RECAP into computer, check compatibility**

**Run the device scanner:**

👉 **<https://recapmycalls.com/audio/>**

This free browser tool scans your computer's audio inputs.

**What you'll see:**

- ✅ **"STEREO input detected (2 channels)"** → Perfect! Continue to Step 4
- ❌ **"MONO input detected (1 channel)"** → You need a USB adapter

**If MONO:**

- Most modern laptops/Macs have MONO-only inputs
- This is NOT a defect - it's a compatibility issue
- Solution: Get Andrea USB stereo adapter ($20-40) FIRST - [See USB Adapter Solution](../troubleshooting/device-scanner.md)
- RECAP works perfectly, your computer just needs the adapter
- **Don't proceed to Step 4 until you have the USB adapter**

**Take a screenshot** of the scanner results - helpful if you need support later.

---

### Step 4: Connect to Computer & Record (2 minutes)

**NOW connect to your computer:**

```
Phone ──→ RECAP ──→ Headset
            │
            └──→ Computer MIC IN (or USB Adapter)
```

**Connection:**

- Use included cable to connect RECAP's MIC output to:
  - **If STEREO input:** Computer's MIC IN port (pink or mic icon)
  - **If MONO input:** USB adapter's MIC IN jack → USB adapter → Computer USB port

**⚠️ Must be MIC IN (not LINE IN)**

> ⚠️ **Unplug from the phone first, then rebuild with the phone LAST.** Don't add the recording cable to a chain that's already plugged into your phone — that's the connection order problem again. Disconnect from the phone, connect headset → RECAP → recording cable, then plug into the phone last. See [Connection Order troubleshooting](../troubleshooting/low-volume-noise.md#problem-audio-routes-to-speaker-or-one-ear-with-lightningusb-c-adapter).

**Open recording software:**

**Windows:**

- Press Windows key, type "sound recorder", press Enter
- Click "Start Recording" button

**Mac:**

- Open QuickTime Player
- File → New Audio Recording
- Click dropdown next to record button → Select "External Microphone"
- Click red record button

**Make a test recording:**

1. Start recording
2. Make a test call (or call voicemail)
3. Say something, have them say something
4. Stop recording
5. Play it back

**What you should hear:**

- ✅ Both sides of conversation (you + them)
- ✅ Clear audio, reasonable volume

**Problems?**

- One-sided or no audio → [Go to Troubleshooting](../troubleshooting/no-audio.md)
- Very quiet audio → [See "Low Volume" solution](../troubleshooting/low-volume-noise.md)

---

**🎉 That's it! You're ready to record calls.**

After first-time setup, it's plug-and-play. Just connect everything and hit record.

---

