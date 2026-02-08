## Compatibility Requirements

### Call Device Compatibility

RECAP works with any device that has a **combo headset port** (3.5mm TRRS) — this includes phones, tablets, and computers.

**Compatible:**

- iPhone (with 3.5mm jack or Lightning/USB-C to 3.5mm adapter)
- Android phones with 3.5mm headphone jack
- Laptops and computers with combo headset jack
- Tablets with 3.5mm headphone jack
- Any device using AHJ standard connector

**Not compatible:**

- Devices without headphone jack and no adapter
- Devices using OMTP standard (rare, mostly older European/Asian models)
- Separate headphone + mic ports (not combo) — these won't pass both signals

**How to check:** If your headset works with the device (you can hear AND be heard), the device is compatible.

---

### Headset Compatibility

**Requirements:**

- Must be compatible with YOUR call device
- Standard 3.5mm TRRS connector (4-pole)
- Known-working headsets: Apple EarPods, most phone headsets

**How to test compatibility:**

1. Plug headset directly into phone (no RECAP)
2. Make test call
3. Verify: Can you hear them? Can they hear you?
4. If both YES → Headset is compatible

**Common incompatibilities:**

- Old headsets using OMTP standard (mic/ground pins reversed)
- Headsets designed for different phone brands
- Damaged or worn-out headsets
- PC gaming headsets (often use different connector types)

**⚠️ Important:** Distance of microphone boom to mouth affects volume. Keep mic 1-2 inches from corner of mouth.

---

### Computer Compatibility

**The Critical Requirement: STEREO Microphone Input**

This is where most compatibility issues occur.

**✅ Compatible:**

- Computers with stereo MIC IN port (2 channels)
- Older Windows laptops/desktops (pre-2015)
- Some desktop PCs with dedicated sound cards
- Computers using USB adapter (Andrea recommended)

**❌ NOT Compatible (without USB adapter):**

- Most modern laptops (2015+) - usually MONO input only
- Most Mac computers - usually MONO input or LINE IN only
- Computers with only LINE IN port (no bias voltage)
- Computers with only headphone/speaker outputs

**How to check:** Visit **<https://recapmycalls.com/audio/>** and run the free device scanner.

**Port types explained:**

| Port Type | Compatible? | How to Identify |
|-----------|-------------|-----------------|
| MIC IN (stereo) | ✅ YES | Pink port or mic icon, supports stereo |
| MIC IN (mono) | ❌ NO - need USB adapter | Pink port but only 1 channel |
| LINE IN | ❌ NO | Blue port, no bias voltage |
| Combo port | ❌ Usually MONO | One port for both headphones + mic |
| Headphone OUT | ❌ NO | Green port, output only |

**Solution for incompatible computers:** Use Andrea USB stereo adapter ($20-40)

---

### Recording Device Compatibility

**Compatible devices:**

- Digital voice recorders with **stereo** external mic input
- Portable recorders (Zoom, Tascam, etc.) with stereo MIC IN
- Professional recorders with stereo line-level input + preamp

**Requirements:**

- Must accept stereo external microphone (2 channels)
- Must provide bias voltage (or use adapter with bias voltage)
- **Not LINE IN** - must be MIC IN or have MIC mode

**How to check your recorder:**

- Look in user manual for "stereo external microphone" support
- Some recorders have mono/stereo switch - must be set to STEREO
- Some have MIC IN / LINE IN switch - must be set to MIC IN

**NOT compatible (without adapter):**

- Voice recorders with only mono mic input
- Devices with only LINE IN (no bias voltage)
- iPhone/iPad/Android directly (combo ports only) — see USB adapter option below

---

### What's NOT Compatible

**❌ LINE IN ports**

- Don't provide bias voltage needed to power RECAP
- Usually blue color or line icon
- Found on: Older desktops, some Macs, stereo equipment

**❌ +48V Phantom Power**

- Professional mixer equipment
- **Will damage RECAP** - never connect to phantom power!
- RECAP designed for computer mic bias only (2V max)

**⚠️ Mobile devices as recorder (requires USB adapter)**

- iPhones, iPads, Android phones/tablets have combo ports only
- RECAP requires stereo MIC IN, which combo ports don't provide
- **Solution:** USB audio adapter with stereo mic input, connected via USB-C or Lightning
- Example: USB-C audio interface with 3.5mm stereo mic input

**❌ Splitter cables**

- No supported configuration for using splitters
- Splitters are for different purpose (sharing audio)

---

