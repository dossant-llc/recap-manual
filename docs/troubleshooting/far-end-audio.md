### Problem: Callers Say I Sound Muffled or Distant

**Symptom:** People on the other end say your voice sounds muffled, distant, far away, or like you're on speakerphone — or they keep asking you to repeat yourself.

> ⚠️ **This page is about the live call, not the recording.** If your *recording* is silent, one-sided, or too quiet, you are on the wrong page — see [No Audio Recorded](no-audio.md) or [Low Volume & Noise](low-volume-noise.md). Those tests examine the recording output, and they cannot grade what your caller hears. (One exception: if your own voice is completely missing from a recording, check both the [headset mic](#cause-1-most-common-no-microphone-on-the-headset-cable) and the recording input; that symptom alone does not establish the cause. See [only one side recorded](no-audio.md#problem-recording-only-has-audio-on-one-side).)

**How to tell which one you have:** if you are repeating what other people told you ("everybody says I sound muffled"), you are on the right page. If you are describing something you played back yourself, you want the recording pages above.

---

### Step 1: Get a measurement you can repeat

"Muffled" is a judgement call, and asking a caller to grade you gives a slightly different answer every time. Use your own voicemail instead — it travels the same microphone path your callers hear, and you can replay it as often as you like.

**To reach your own voicemail:** dialling your own number from your own phone usually drops you into your mailbox rather than your greeting. Instead, call your carrier's voicemail access number and use the "leave a message" option, or call a second phone you own and let it ring through to voicemail.

Then, at each rung below:

1. Leave a short message — ten seconds is plenty, and **say the same sentence every time**
2. Play it back through the same headset
3. Note how it sounds compared with the previous rung

> **Read it as a comparison, not a verdict.** Voicemail is compressed, so it always sounds a little duller than a live call — even on a perfectly healthy setup. Don't judge one recording against how a live call sounds. What matters is whether a rung sounds **worse than the rung before it**.

---

### Step 2: The three-rung ladder

Add exactly **one** link to the chain per rung, and leave a voicemail after each. Adding two at once tells you nothing about which one caused it.

> ⚠️ **Rung 1 only counts if you physically unplug RECAP and make a new call.** If you're answering from what you already know about your setup, you're answering rung 2. This is the single most common reason this goes in circles.

| Rung | What's connected | If it sounds worse at this rung |
|------|------------------|---------------------------------|
| **1** | Headset → phone. RECAP completely out of the chain. | This baseline symptom occurs with RECAP absent; it does not explain any additional degradation when RECAP or the recording path is added. Check headset/app routing and call conditions. Check [Cause 1: the headset microphone](#cause-1-most-common-no-microphone-on-the-headset-cable), then [Cause 2: the adapter](#cause-2-the-adapter-doesnt-carry-the-microphone-channel). |
| **2** | Headset → RECAP → phone. Nothing in RECAP's MIC jack. | See [Cause 3: connection order](#cause-3-connection-order), and check the headset is in the pass-through jack rather than the MIC jack. |
| **3** | Headset → RECAP → phone, **plus** the recording cable in RECAP's MIC jack. **Rebuild the whole chain and plug the phone in LAST** — don't just add the cable to what's already connected, or you'll break the connection order and get a misleading result. | The recording connection introduces the observed change; see [Cause 4 checks](#cause-4-wrong-jack-or-the-wrong-recording-cable) without treating them as a verdict. |

**Sounds the same at every rung?** No added degradation was observed in that comparison. Call quality, signal strength, the room or the other line may be involved; an unchanged comparison does not certify every part or exclude intermittent behavior. Try the same test on a different phone or in a different location. If callers still say you sound muffled on a chain that tests clean at all three rungs, [contact support](../support.md) and say exactly that.

---

### Cause 1 (most common): no microphone on the headset cable

RECAP is a passive splitter. It can only pass along audio that physically travels through its cable. If your headset has no microphone **on the cable**, your voice never enters the chain — your call device uses its own built-in microphone instead. That microphone may be lying on your desk while you are wearing the headset, so you can come across as distant.

The confusing part: your phone does this with *any* mic-less headset, so swapping one mic-less headset for another changes nothing, and it starts to look like a device fault when it isn't.

**How to check:** look along the headset cable for a boom arm, or a small inline blob partway down the wire (often with the volume buttons). That blob is the microphone. No boom and no blob means no microphone on the cable.

**These cannot work with RECAP:**

| Headset type | Why not | What you'd see |
|--------------|---------|----------------|
| Listening-only earphones (3-pole TRS plug) | No microphone on the cable. Common with music earphones and audiophile IEMs, which often ship with a mic-less cable. | Call audio works, and recordings capture the caller but **not you** |
| USB headsets | Connect digitally. RECAP taps the analog 3.5mm signal, so a USB headset never passes through it. | RECAP is bypassed entirely |
| Lightning or USB-C EarPods | Have their own converter built into the plug, so they connect straight to the phone and bypass RECAP. | RECAP is bypassed entirely |
| Bluetooth / wireless headsets | Nothing travels down a cable for RECAP to tap. | RECAP is bypassed entirely |

**The fix:** a wired 3.5mm headset with a microphone on the cable (a 4-pole TRRS plug). Apple's **3.5mm** EarPods are a widely available known-good reference. See [Headset Compatibility](../getting-started/requirements.md#headset-compatibility) — a small number of TRRS headsets use a reversed pinout or an unusual connector and still misbehave, which is why a known-good headset is the fastest way to rule this out.

---

### Cause 2: the adapter doesn't carry the microphone channel

If your phone has no headphone jack, there is a Lightning or USB-C to 3.5mm adapter in your chain — and it is still there at rung 1, because rung 1 only removes RECAP. Many inexpensive adapters pass audio to your ears but don't carry the microphone channel back. The result is the same as Cause 1: the phone falls back to its own built-in microphone.

**How to check:** try a different adapter, ideally one from the tested list — <https://recapmycalls.com/compatible-adapters-for-recap/> — and repeat the rung 1 voicemail.

---

### Cause 3: connection order

Your phone decides how to route audio at the instant something is plugged in. If the headset is not already in the chain when the phone sees the adapter, the phone can lock into the wrong routing mode and leave your microphone on the wrong path.

**Connect in this order, every time:**

1. Headset into RECAP's headset jack
2. Recording cable into RECAP's MIC jack (if you're recording)
3. RECAP into the Lightning/USB-C adapter
4. Adapter into the phone **last**

Full explanation and the iPhone reset path: [Audio Routes to Speaker or One Ear with Lightning/USB-C Adapter](low-volume-noise.md#problem-audio-routes-to-speaker-or-one-ear-with-lightningusb-c-adapter).

---

### Cause 4: wrong jack, or the wrong recording cable

This one only shows up at rung 3 — fine without the recording cable, worse with it. That comparison localizes a change introduced when the recording connection is added; it does not establish the cause. A wrong jack or cable is one possibility. The unit, recorder/input loading, contact or grounding interaction also remains possible until isolated. Start with two visible checks:

1. **The recording cable is in RECAP's MIC jack**, not the headset pass-through jack.
2. **The recording cable is the 3-pole (TRS) cable that ships in the box.** Count the black bands on the plug: **2 bands = TRS (correct), 3 bands = TRRS (wrong)**. A 4-pole cable looks close enough to be missed, but it can ground on the wrong conductor — most often showing up as a unit that appears dead, or a recording missing your voice. If you swapped in your own cable, repeat with the boxed TRS cable as a controlled comparison; a changed result localizes that cable/connection combination rather than proving the unit's condition.

If the jacks and TRS cable are correct and rung 3 still degrades the call, note
which recorder/input is connected and the comparison result, then [contact support](../support.md).
Support can help isolate the recording path, including unit behavior and loading;
this result alone does not justify buying another cable, adapter or recorder.

---

### Still worse at rung 1?

Rung 1 has RECAP completely out of the chain, so a symptom present there also occurs without RECAP. Check headset/adapter routing and call conditions; that baseline alone does not explain an additional change at rung 2 or 3. Work through [Cause 1](#cause-1-most-common-no-microphone-on-the-headset-cable) and [Cause 2](#cause-2-the-adapter-doesnt-carry-the-microphone-channel) first.

If you've confirmed there's a microphone on the headset cable and tried a known-good adapter and rung 1 is still worse, [contact support](../support.md) and tell us **which rung number** it first got worse at, your headset make and model, and which adapter is in the chain. That saves several rounds of back-and-forth.

---
