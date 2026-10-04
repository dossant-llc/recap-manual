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

> **No headphone jack on your phone?** You need a Lightning or USB-C to 3.5mm adapter — and it has to be one that carries the microphone channel. Many cheap adapters do not, which leaves your phone using its own built-in microphone. Tested adapters: <https://recapmycalls.com/compatible-adapters-for-recap/>

---

### Headset Compatibility

> ⚠️ **The one rule that matters most: the microphone has to be on the headset cable.**
>
> RECAP is a passive splitter — it can only work with audio that physically travels through its cable. If your headset has no microphone on the cable, your voice never enters the chain: your call device uses its own built-in microphone instead. Your recording will be missing your side, and your callers may hear you as distant, since that microphone can be sitting on your desk while you wear the headset.
>
> **How to check:** look along the cable for a boom arm, or a small inline blob partway down the wire (often with the volume buttons). That blob is the microphone. No boom and no blob means no microphone on the cable.

**Requirements:**

- Wired, with a microphone **on the cable** — a 3.5mm TRRS plug (4-pole)
- Must be compatible with YOUR call device
- Known-working headsets: Apple **3.5mm** EarPods, most phone headsets

A mic on the cable is the first requirement, and an inexpensive headset can meet it — the headset does not shape how your *caller* sounds in the recording, since that audio comes from the call itself. Headset quality still affects how **you** sound, though: a weak or noisy microphone shows up on your own channel. And a small number of TRRS headsets use a reversed pinout or an unusual connector and still misbehave — see **Common incompatibilities** below.

**These cannot work with RECAP:**

| Headset type | Why not | What you'd see |
|--------------|---------|----------------|
| Listening-only earphones (3-pole TRS plug) | No microphone on the cable. Common with music earphones and audiophile IEMs, which often ship with a mic-less cable. | Call audio works, and recordings capture the caller but **not you** |
| USB headsets | Connect digitally. RECAP taps the analog 3.5mm signal, so a USB headset never passes through it. | RECAP is bypassed entirely |
| Lightning or USB-C EarPods | Have their own converter built into the plug, so they connect straight to the phone and bypass RECAP. | RECAP is bypassed entirely |
| Bluetooth / wireless headsets | Nothing travels down a cable for RECAP to tap. | RECAP is bypassed entirely |

**How to test compatibility:**

First confirm the **microphone is on the cable** (see the box above). A headset with no mic on the cable still passes the call test below, because your phone quietly falls back to its own built-in microphone. So the call test alone can't tell you the headset will work with RECAP.

1. Plug headset directly into phone (no RECAP)
2. Make test call
3. Verify: Can you hear them? Can they hear you?
4. If both YES **and** the mic is on the cable → Headset is compatible

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
- Computers using a USB adapter that adds a stereo mic input

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

**Solution for incompatible computers:** a USB adapter that adds a **stereo** microphone input. Current recommended models are kept on the [compatible adapters guide](https://recapmycalls.com/compatible-adapters-for-recap/) — that list is maintained as hardware changes, so check it there rather than relying on a model name in this manual.

---

### Recording Device Compatibility

**Compatible devices:**

- Digital voice recorders with a **stereo** external mic input that supplies plug-in power
- Portable/field recorders meeting the same two conditions

We don't certify individual recorder models — there are too many to test, and a
model that works in one firmware revision may not in the next. Check your own
recorder against the two conditions below; its manual is the only reliable source.

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

