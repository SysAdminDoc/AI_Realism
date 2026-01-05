# AI Video Production Handbook
### From Still Image to Photorealistic Video in 2026

---

## 🎯 Quick Start: Which Workflow Do You Need?

| I want to... | Jump to |
|:---|:---|
| Turn a photo into a talking video | [The Core Pipeline](#-phase-1-the-image) → [Motion Control](#-kling-motion-control) → [Lip Sync](#-lip-synchronization) |
| Make a music video | [Multi-Angle Technique](#multi-angle-music-video-workflow) |
| Clone my voice for narration | [Voice Cloning](https://github.com/SysAdminDoc/AI_Realism?tab=readme-ov-file#%EF%B8%8F-voice-cloning) |
| Fix a failed generation | [Repair & Salvage](#-repair--salvage) |
| Understand what tools to use | [Tool Selector](https://github.com/SysAdminDoc/AI_Realism?tab=readme-ov-file#%EF%B8%8F-tool-selector-by-task) |

---

# Part 1: The Production Pipeline

> **The 80/20 Rule:** Your source image determines 80% of your final quality. Everything downstream is damage control.

<img width="2816" height="534" alt="Gemini_Generated_Image_mmku42mmku42mmku" src="https://github.com/user-attachments/assets/f6aa214f-a87e-45a9-8b24-2f53c2d42436" />

---

## 📸 Phase 1: The Image

### Tool Selector

| Tool | Best For | Link |
|:---|:---|:---|
| **Flux 2 Pro** | Photorealism, fine detail | [flux.ai](https://flux.ai) |
| **Midjourney v7** | Artistic interpretation, cultural references | [midjourney.com](https://www.midjourney.com) |
| **Ideogram 3.0** | Text rendering in images | [ideogram.ai](https://ideogram.ai) |
| **Leonardo AI** | Variations, consistency | [leonardo.ai](https://leonardo.ai) |

> 📺 **Tutorial:** [Midjourney V7 Complete Guide](https://docs.midjourney.com/hc/en-us/articles/32199405667853-Version) — Official documentation for V7 features including Draft Mode and Omni Reference

### Prompt Formula

<img width="2816" height="561" alt="Gemini_Generated_Image_cqcdwscqcdwscqcd" src="https://github.com/user-attachments/assets/aeb57517-6bd8-4e9c-8942-1a7b15fa360d" />

**Example:**
```
Woman in red dress answering phone, annoyed expression, 
shallow focus, practical lighting, 35mm film grain, hotel lobby
```

> ⚠️ **Common Mistake:** Long environment descriptions. Keep it minimal — complex backgrounds create animation problems later.

### Before You Animate: The NanoBanana Pass

If a face looks "almost right" but something's off, fix it NOW. Motion amplifies every flaw.

**NanoBanana** ([nanobanana.com](https://www.nanobanana.com)) corrects:
- Facial proportions without changing identity
- Eye alignment and asymmetry
- Mouth/jawline for animation readiness

```
Image Generation → NanoBanana (1 pass only) → Animation
```

> 💡 **Pro Tip:** One pass only. Multiple passes flatten expression.

---

## 🎬 Phase 2: Animation

### Quick Decision Guide

| Your Shot Needs... | Use This |
|:---|:---|
| Precise body movement from reference video | **Kling Motion Control** |
| Dialogue with built-in audio | **Google Veo 3.1** |
| Physical weight and grounded movement | **Hailuo Minimax** |
| Fast turnaround, good physics | **Luma Dream Machine** |
| Style transformation of real footage | **Runway Gen-4** |
| Long-form narrative coherence | **OpenAI Sora 2** |

### Platform Links

| Platform | Link |
|:---|:---|
| Kling AI | [klingai.com](https://klingai.com) |
| Google Veo | [deepmind.google/veo](https://deepmind.google/technologies/veo/) |
| Hailuo/Minimax | [hailuoai.video](https://hailuoai.video) |
| Luma Dream Machine | [lumalabs.ai](https://lumalabs.ai/dream-machine) |
| Runway | [runwayml.com](https://runwayml.com) |
| OpenAI Sora | [openai.com/sora](https://openai.com/sora) |
| Pika Labs | [pika.art](https://pika.art) |

---

## 🎭 Kling Motion Control

**What it does:** Transfer your recorded performance onto any character. Your body drives their body.

> 📺 **Official Guide:** [Kling Motion Control User Guide](https://app.klingai.com/global/quickstart/motion-control-user-guide)
> 
> 📺 **Deep Dive:** [Higgsfield Motion Control Guide](https://higgsfield.ai/blog/Kling-2.6-Motion-Control-Full-Guide)

### The 60-Second Setup

1. **Record yourself** (3-30 sec, stationary camera, single person)
2. **Upload reference video** (your performance)
3. **Upload character image** (who you want to become)
4. **Choose mode:**
   - *Exact* = Static camera, precise match
   - *Partial* = Camera can move independently
5. **Generate**

### Critical Rules

| Do | Don't |
|:---|:---|
| ✅ Match framing (waist-up reference → waist-up output) | ❌ Full-body reference for close-up output |
| ✅ Empty hands in character image | ❌ Hold props (they disappear) |
| ✅ Neutral mouth in character image | ❌ Open mouth or teeth showing |
| ✅ Single subject only | ❌ Multiple people |
| ✅ Stationary camera | ❌ Pans, zooms, handheld shake |

### Multi-Angle Music Video Workflow

Turn one performance into a multi-camera edit:

```
1. Record ONE continuous performance
          ↓
2. Generate 3-5 character images (different angles/backgrounds)
          ↓
3. Run SAME reference video against EACH image
          ↓
4. All outputs sync perfectly (they share timing)
          ↓
5. Edit together with beat-matched cuts
```

> 💡 **Pro Tip:** Segment into 10-second chunks. Generate all angles before editing.

---

## 👄 Lip Synchronization

### Tool Selector

| Tool | Best For | Link |
|:---|:---|:---|
| **Kling Lip Sync** | Integrated with motion, handles singing | [Built into Kling AI](https://app.klingai.com/global/video-to-lip/new) |
| **Magic Hour** | Highest realism, extreme poses | [magichour.ai](https://magichour.ai) |
| **HeyGen** | Avatars, multilingual | [heygen.com](https://www.heygen.com) |
| **Sync.so** | Style learning, dialogue editing | [sync.so](https://sync.so) |

### The Workflow

```
Generate video (face visible, 5-10 sec)
          ↓
Isolate vocals from audio (Lalal.ai or Moises.ai)
          ↓
Apply lip sync tool
          ↓
Recombine with instrumental in editor
```

> ⚠️ **Never** feed a full music track to lip sync. Isolate vocals first. [Ultimate Vocal Removal](https://ultimatevocalremover.com/) is incredible and free.

### Kling Lip Sync Steps

1. Generate base video with visible face
2. Enable "Match Mouth" tracking (~10 min processing)
3. Upload clean isolated vocal audio
4. Adjust frame offset in your editor if needed

---

## 🎙️ Voice Cloning

### Quick Comparison

| Platform | Best For | Free Tier | Pro Price | Link |
|:---|:---|:---|:---|:---|
| **ElevenLabs** | Emotional range, English | 10K chars/mo | $22/mo | [elevenlabs.io](https://elevenlabs.io) |
| **Fish Audio** | Emotion control, multilingual | Limited | $5-330 | [fish.audio](https://fish.audio) |
| **Play.ht** | 100+ languages | Limited | $14-198 | [play.ht](https://play.ht) |
| **Resemble AI** | API access, enterprise | Pay-as-you-go | $29-99 | [resemble.ai](https://www.resemble.ai) |
| **Respeecher** | Film industry standard | None | ~$167/mo | [respeecher.com](https://www.respeecher.com) |

> 📺 **Tutorial:** [ElevenLabs Voice Cloning Guide](https://elevenlabs.io/docs/product-guides/voices/voice-cloning) — Official documentation for instant and professional voice cloning

### Quick Start with ElevenLabs

1. Record 1-3 minutes of clean audio (no background noise)
2. Upload to Voices → Create Voice → Instant Clone
3. For pro quality: 30+ minutes audio, use Professional Clone (Creator plan required)

> ⚠️ **Legal:** Get written consent for any voice you clone commercially.

---

## 🎵 Music Generation

| Platform | Best For | Link |
|:---|:---|:---|
| **Suno v4.5** | Complete songs with vocals, easiest | [suno.com](https://suno.com) |
| **Udio** | Stem control, pro mixing | [udio.com](https://www.udio.com) |

> 📺 **Tutorial:** [Suno Complete Guide](https://suno.com/hub/how-to-make-a-song) — Official guide to creating AI music

### Workflow for Video

```
Describe song style in Suno
          ↓
Generate with isolated stems enabled
          ↓
Feed vocal stem to lip sync
          ↓
Recombine in Video Editor
```

---

## 📈 Phase 3: Upscaling & Finishing

### Topaz Video AI Settings

| Setting | Value | Why |
|:---|:---|:---|
| Model | Proteus | Best for AI-generated content |
| Output | 4K (3840×2160) | Distribution standard |
| **Recover Detail** | **0** | ⚠️ Non-zero causes face morphing |

> 📺 **Tutorial:** [Topaz Video AI Documentation](https://docs.topazlabs.com/video-ai/filters/enhancement)

**Link:** [topazlabs.com/topaz-video](https://www.topazlabs.com/topaz-video)

### Film Grain Overlay (The Unity Trick)

Different AI clips have different textures. Grain unifies everything.

```
In DaVinci Resolve:
1. Place grain asset above all footage
2. Blend mode: Overlay
3. Opacity: ~30%
```

This single step often does more than hours of per-clip color correction.

---

# Part 2: Optimization & Troubleshooting

## 💰 Credit Efficiency

### The Golden Rule

```
Lock framing → Test at low tier → Generate at full quality → Upscale ONCE → Lip sync LAST
```

Reordering these steps wastes money on content that gets regenerated.

### Money-Saving Tactics

- ✅ Generate at native resolution, upscale once at the end
- ✅ Test complex shots with Standard mode before Professional
- ✅ Batch similar shots before committing
- ❌ Don't use platform "enhancers" (Topaz is better and cheaper per clip)
- ❌ Don't lip sync before final framing is locked

---

## 🔧 Repair & Salvage

A "failed" generation is often fixable. Repair costs time; regeneration costs credits.

### Motion Repair Tools

| Tool | Fixes | Link |
|:---|:---|:---|
| **FlowFrames** | Optical flow smoothing | [github.com/n00mkrad/flowframes](https://github.com/n00mkrad/flowframes) |
| **Topaz Chronos** | Frame pacing | Included in Topaz Video AI |
| **FaceFusion** | Temporal face stabilization | [github.com/facefusion/facefusion](https://github.com/facefusion/facefusion) |
| **EbSynth** | Style locking across frames | [ebsynth.com](https://ebsynth.com) |

### Repair vs Regenerate Decision

| Symptom | Action |
|:---|:---|
| Isolated jitter, content is good | Repair |
| Uneven frame pacing | Repair |
| Wrong physics, identity drift | Regenerate |
| Multiple compounding issues | Regenerate |

---

## 🚨 Common Failures & Fixes

| What You See | What Caused It | Fix |
|:---|:---|:---|
| Teeth morph mid-sentence | Aggressive lip sync | Reduce lip sync strength |
| Floating hands | Reference video framing mismatch | Re-crop reference to match output |
| Eye jitter | Face too small in frame | Generate with larger face |
| Texture crawl | Sharpening or HDR/SDR mixing | Disable sharpening, unify color space |
| Identity drift | Inconsistent reference images | Use Omni Reference for consistency |
| Background loops | Clip too long | Keep under 10 seconds |

---

## ✅ Quality Control Checklist

Run before final export. If anything fails, regenerate — don't patch.

### Visual
- [ ] Eyes track consistently, no micro-jumps
- [ ] Teeth stable across frames
- [ ] Hands don't partially disappear
- [ ] Clothing doesn't shimmer or crawl
- [ ] Background motion doesn't loop

### Audio
- [ ] Hard consonants (p, b, t, d) match lips
- [ ] Breathing matches chest movement
- [ ] Room tone matches environment size

### Editorial
- [ ] Every cut has purpose
- [ ] Camera movement has intent
- [ ] Emotional state clear within 2 seconds

---

# Part 3: Pre-Production & Organization

## 📋 Previsualization

Teams that storyboard before generation report **30-50% fewer regenerations**.

### Storyboarding Tools

| Tool | Capability | Link |
|:---|:---|:---|
| **Boords** | Text-to-storyboard, shot continuity | [boords.com](https://boords.com) |
| **Shotry AI** | AI storyboards with camera metadata | [shotry.ai](https://shotry.ai) |
| **Kive.ai** | Visual reference boards | [kive.ai](https://kive.ai) |

### Before Generating Anything

1. Define camera angle, lens, movement intent
2. Create reference boards for color/lighting
3. Map shot sequence with emotional purpose
4. Test with still images before video

---

## 📁 Project Structure

```
Project/
├─ 01_Source_Images/
├─ 02_Reference_Video/
├─ 03_Generations/
│  ├─ v1_exploration/
│  ├─ v2_selected/
│  └─ v3_final/
├─ 04_Audio/
├─ 05_Upscaled/
├─ 06_Edit/
└─ prompts.txt
```

> ⚠️ **Never overwrite generations.** Version drift is how quality regressions sneak in.

---

## 🎨 Camera Science Emulation

AI output is mathematically perfect. Real footage isn't. Add controlled imperfection.

| Tool | What It Does | Link |
|:---|:---|:---|
| **Dehancer Pro** | Film response curves | [dehancer.com](https://www.dehancer.com) |
| **FilmBox** | Color science emulation | [videovillage.co/filmbox](https://videovillage.co/filmbox/) |
| **CineMatch** | Camera-to-film matching | [filmconvert.com/cinematch](https://www.filmconvert.com/cinematch) |

Apply after generation, before final grade. Adds halation, grain, highlight rolloff.

---

# Part 4: Technical Standards

## 🎞️ Color & Frame Rate

### Color Space
- Assume **Rec.709 gamma 2.4** unless platform specifies otherwise
- Convert all clips to single working space before editing
- Never mix HDR and SDR without tone mapping

### Frame Rate
- Generate everything at **24fps or 30fps**, never mixed
- Fix frame rate BEFORE lip sync, never after
- If jittery, apply optical flow AFTER upscaling

---

## 📱 Surviving Social Compression

### High-Risk Elements (Will Look Bad After Compression)
- Fine skin texture
- Subtle gradients
- Neon lighting
- Fog, smoke, rain

### Defense
- Add light grain before export (gives encoders texture to preserve)
- Boost contrast slightly
- Avoid pure black backgrounds (macroblock badly)
- Export at higher bitrate than platform recommends

---

# 🛠️ Tool Selector by Task

## Image Generation
| Tool | Link |
|:---|:---|
| Flux 2 Pro | [flux.ai](https://flux.ai) |
| Midjourney v7 | [midjourney.com](https://www.midjourney.com) |
| Ideogram 3.0 | [ideogram.ai](https://ideogram.ai) |
| Leonardo AI | [leonardo.ai](https://leonardo.ai) |

## Image Enhancement
| Tool | Link |
|:---|:---|
| NanoBanana | [nanobanana.com](https://www.nanobanana.com) |
| Enhancer.ai | [enhancer.ai](https://enhancer.ai) |
| Topaz Photo AI | [topazlabs.com/topaz-photo-ai](https://www.topazlabs.com/topaz-photo-ai) |
| Topaz Gigapixel | [topazlabs.com/gigapixel](https://www.topazlabs.com/gigapixel) |

## Video Animation
| Tool | Link |
|:---|:---|
| Kling AI | [klingai.com](https://klingai.com) |
| Google Veo | [deepmind.google/veo](https://deepmind.google/technologies/veo/) |
| Hailuo Minimax | [hailuoai.video](https://hailuoai.video) |
| Luma Dream Machine | [lumalabs.ai/dream-machine](https://lumalabs.ai/dream-machine) |
| Runway Gen-4 | [runwayml.com](https://runwayml.com) |
| OpenAI Sora | [openai.com/sora](https://openai.com/sora) |
| Pika Labs | [pika.art](https://pika.art) |
| Morph Studio | [morphstudio.com](https://www.morphstudio.com) |
| Kaiber | [kaiber.ai](https://kaiber.ai) |

## Lip Sync
| Tool | Link |
|:---|:---|
| Magic Hour | [magichour.ai](https://magichour.ai) |
| HeyGen | [heygen.com](https://www.heygen.com) |
| Sync.so | [sync.so](https://sync.so) |
| LipDub AI | [lipdub.ai](https://lipdub.ai) |

## Voice & Audio
| Tool | Link |
|:---|:---|
| ElevenLabs | [elevenlabs.io](https://elevenlabs.io) |
| Fish Audio | [fish.audio](https://fish.audio) |
| Play.ht | [play.ht](https://play.ht) |
| Lalal.ai (stem separation) | [lalal.ai](https://www.lalal.ai) |
| Moises.ai (stem separation) | [moises.ai](https://moises.ai) |

## Music Generation
| Tool | Link |
|:---|:---|
| Suno | [suno.com](https://suno.com) |
| Udio | [udio.com](https://www.udio.com) |

## Video Upscaling & Repair
| Tool | Link |
|:---|:---|
| Topaz Video AI | [topazlabs.com/topaz-video](https://www.topazlabs.com/topaz-video) |
| FlowFrames | [github.com/n00mkrad/flowframes](https://github.com/n00mkrad/flowframes) |
| FaceFusion | [github.com/facefusion/facefusion](https://github.com/facefusion/facefusion) |
| EbSynth | [ebsynth.com](https://ebsynth.com) |

## Aggregators (Multi-Tool Access)
| Tool | Link |
|:---|:---|
| Higgsfield | [higgsfield.ai](https://higgsfield.ai) |
| Freepik AI | [freepik.com/ai](https://www.freepik.com/ai) |

---

# 🎯 Durable Principles

Tools change monthly. These don't:

1. **Capture quality determines your ceiling.** No tool compensates for bad inputs.

2. **Lock framing early.** Mid-process reframing cascades problems everywhere.

3. **Modular separation.** Treat body motion, face animation, and voice as independent tracks. Combine in editorial.

4. **Regeneration beats repair.** Fresh output usually costs less than fixing broken output.

5. **Ambiguity multiplies cost.** Know exactly what you want before generating.

---

*Last verified: January 2026*
*Platform capabilities shift rapidly — confirm current features before production.*
