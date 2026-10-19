## Compatibility Requirements

### Compatibility checklist

Use a **call device (CALL)** and a **separate recording device (REC)**. Check the
connection and input specifications, rather than a product name or headphone jack alone.

| Part | What to check |
|---|---|
| CALL phone/device | A 3.5 mm AHJ/CTIA TRRS headset connection, directly or through a microphone-capable adapter |
| Phone adapter | Correct Lightning/USB-C connector **and microphone input support**; a headphone-only adapter cannot carry your headset mic |
| Headset | Wired 3.5 mm **TRRS, 4 contacts / 3 insulating bands**, with an inline or boom microphone; it must work on CALL with the same adapter |
| Recording cable | Included 3.5 mm male-to-male **TRS, 3 contacts / 2 insulating bands**, straight-through stereo cable; a TRRS headset cable is a different part |
| REC input | External **stereo microphone input (two channels)**; MIC mode where selectable, with plug-in power enabled where supported; no phantom power |
| Recording settings | Select the connected external input, record both channels separately, and turn off mono mixing and processing for the initial test |
| Calling app | Call audio and the headset microphone must both route through the wired headset path, including in apps such as Teams |

**Before an important call:** follow [setup and the two-sided test](../using-recap/making-calls.md#setup-and-two-sided-test).
For recorder details and the open electrical-validation issue, see
[Recording Device Compatibility](#recording-device-compatibility).

### What a compatibility claim means

A **physically tested configuration** needs a recorded test for those exact models
and settings. A tested phone adapter does not validate every phone, app or recorder
used with it. A **specification-based expectation** means the manufacturer's manual
matches the requirements; it is useful evidence, but not certification or a guarantee
for the whole chain. If the evidence is missing, compatibility is unresolved.

If our setup instructions are unclear or the documented setup fails, [contact support](../support.md)
with the specific question or symptom. We can help isolate the RECAP setup; you do not
need a full device inventory for a general requirements question.

### Call Device Compatibility

RECAP uses the call device's **AHJ/CTIA combo headset connection** (3.5mm TRRS). Phones, tablets and computers may provide it directly or through a compatible microphone-capable adapter; the app must actually route both call audio and the headset microphone through it.

**Connection types to check:**

- iPhone (with 3.5mm jack or Lightning/USB-C to 3.5mm adapter)
- Android phones with 3.5mm headphone jack
- Laptops and computers with combo headset jack
- Tablets with 3.5mm headphone jack
- Any device using AHJ standard connector

**Not compatible:**

- Devices without headphone jack and no adapter
- Devices using OMTP standard (rare, mostly older European/Asian models)
- Separate headphone + mic ports (not combo) — these won't pass both signals

**How to check:** Test the headset directly on CALL, using the same phone adapter and calling app. Hearing and being heard through the headset establishes that baseline; then repeat with RECAP and REC in the [two-sided test](../using-recap/making-calls.md#setup-and-two-sided-test).

> **No headphone jack on your phone?** You need a Lightning or USB-C to 3.5mm adapter — and it has to be one that carries the microphone channel. Many cheap adapters do not, which leaves your phone using its own built-in microphone. Adapter guide (check the evidence for the exact model): <https://recapmycalls.com/compatible-adapters-for-recap/>

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
- Reference headset: Apple **3.5mm** EarPods. Other phone headsets must meet the same microphone and pinout requirements; a category name is not a test result.

A mic on the cable is the first requirement, and an inexpensive headset can meet it — the headset does not shape how your *caller* sounds in the recording, since that audio comes from the call itself. Headset quality still affects how **you** sound, though: a weak or noisy microphone shows up on your own channel. And a small number of TRRS headsets use a reversed pinout or an unusual connector and still misbehave — see **Common incompatibilities** below.

**These cannot work with RECAP:**

| Headset type | Why not | What you'd see |
|--------------|---------|----------------|
| Listening-only earphones (3-pole TRS plug) | No microphone on the cable. Common with music earphones and audiophile IEMs, which often ship with a mic-less cable. | Call audio works, and recordings capture the caller but **not you** |
| USB headsets | Connect digitally. RECAP taps the analog 3.5mm signal, so a USB headset never passes through it. | RECAP is bypassed entirely |
| Lightning or USB-C EarPods | Have their own converter built into the plug, so they connect straight to the phone and bypass RECAP. | RECAP is bypassed entirely |
| Bluetooth / wireless headsets | Nothing travels down a cable for RECAP to tap. | RECAP is bypassed entirely |

**How to test compatibility:**

A physical microphone on the cable and a call where both people can hear each
other do **not** establish that the wired mic is active: CALL may still use its
built-in mic. Follow the canonical [physical microphone-routing check and two-sided
test](../using-recap/making-calls.md#setup-and-two-sided-test), using the same adapter
and calling app. Confirm the wired mic route before adding RECAP, then verify the
complete recording path. These results apply to the tested configuration.

**Common incompatibilities:**

- Old headsets using OMTP standard (mic/ground pins reversed)
- Headsets designed for different phone brands
- Damaged or worn-out headsets
- PC gaming headsets (often use different connector types)

**⚠️ Important:** Distance of microphone boom to mouth affects volume. Keep mic 1-2 inches from corner of mouth.

---

### Computer Compatibility

**REC needs a stereo microphone input, not just stereo headphone output.**
Computer age, port color and the word "stereo" in a product listing do not establish
that its **input** captures two channels. A combo headset jack carries stereo
headphone output plus a mono microphone input; it cannot directly capture S2's two
recording channels. A headphone output cannot record at all.

Use the [Audio Device Scanner](https://recapmycalls.com/audio/) to check the selected
input's reported channel capability. It does not measure plug-in power, prove a
signal is present, or certify the complete chain. Confirm capture with the
[two-sided test](../using-recap/making-calls.md#setup-and-two-sided-test).

| Input | RECAP recording setup |
|---|---|
| External stereo MIC input | Use MIC mode and plug-in power where supported; record two channels |
| Mono MIC / combo headset input | Cannot preserve both S2 channels directly |
| Line-only input | Outside the supported MIC setup; not validated here |
| Headphone/speaker output | Output only, cannot capture audio |

If the computer lacks the required input, use an interface that supplies an actual
**stereo microphone input**, not merely stereo playback. See the
[compatible adapters guide](https://recapmycalls.com/compatible-adapters-for-recap/)
and the exact model's manufacturer documentation.

---

### Recording Device Compatibility

Digital voice recorders and portable/field recorders are candidates when their
**external input** meets these checks. A stereo built-in microphone does not prove
that an external jack accepts stereo.

- **3.5 mm TRS stereo external microphone input** with two captured channels.
- **MIC mode**, if the jack switches between mic and line; retain the supported
  **plug-in-power** setup, enabled where selectable.
- Select the external input and **stereo** recording, preserving both channels.
  Disable mono mixing, noise reduction and automatic processing for the test.
- Use the included **TRS recording cable**, not a TRRS headset cable.
- **Never connect RECAP to 48 V phantom power.** A single balanced XLR/TRS input
  is not a stereo microphone input, even if it has three contacts.

Check the exact model's manufacturer manual, then make the
[two-sided test recording](../using-recap/making-calls.md#setup-and-two-sided-test).
A phone's Lightning/USB-C headphone adapter normally exposes a combo headset input,
not this stereo recording input. Using a second mobile device as REC requires a
stereo microphone interface supported by that device and recording app; a connector
adapter alone is insufficient.

#### Plug-in power and voltage: validation pending

Earlier versions of this manual said recorder bias powers S2 and specified a **2 V
maximum**. That explanation and limit were not adequately supported. Review of the
archived **S2 v40** fabrication artwork shows a passive resistor/capacitor circuit
with a series coupling capacitor on **each** recording channel. This conflicts
with the earlier DC-power explanation. Revision applicability and bench validation
remain open; we have not established a validated S2 interface voltage range.

Keep the documented stereo MIC-mode / plug-in-power setup while validation is
pending. A capacitor's **10 V component rating does not establish a 10 V safe
interface limit**, and this correction does not validate line-only inputs or higher
voltages. Do not connect phantom power.

For example, the [Zoom H1essential manual](https://zoomcorp.com/manuals/h1essential-en/)
specifies a stereo mini input, 2 kΩ impedance and 2.5 V plug-in power. The
[H4essential manual](https://zoomcorp.com/manuals/h4essential-en/) specifies a stereo
mini input, at least 2 kΩ and selectable plug-in power, without establishing its
voltage. These are **specification-based candidates**, subject to the open S2
interface validation. No exact-model RECAP physical test or complete iPhone/Teams
chain test has been established for these examples. They are not certified setups.

---

### What's NOT Compatible

**❌ LINE IN ports**

- Outside the supported external stereo MIC setup; line-only operation is not validated here
- Usually blue color or line icon
- Found on: Older desktops, some Macs, stereo equipment

**❌ +48V Phantom Power**

- Professional mixer equipment
- **Never connect RECAP to phantom power.** It is different from microphone plug-in power.
- See the [pending voltage validation](#plug-in-power-and-voltage-validation-pending); no numerical S2 interface limit is established here.

**⚠️ Mobile devices as recorder (requires USB adapter)**

- iPhones, iPads, Android phones/tablets have combo ports only
- RECAP requires stereo MIC IN, which combo ports don't provide
- **Solution:** USB audio adapter with stereo mic input, connected via USB-C or Lightning
- Example: USB-C audio interface with 3.5mm stereo mic input

**❌ Splitter cables**

- No supported configuration for using splitters
- Splitters are for different purpose (sharing audio)

---

