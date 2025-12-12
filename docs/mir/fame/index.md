---
layout: default
title: "FAME"
---

[<< Back to MIR Projects](/mir-riize-homepage/mir/)

# Fame — a MIR Analysis

<br>

This project started out of my interest in Music Information Retrieval and, of course, my love for RIIZE’s music. So I figured: why not look at their tracks through an MIR lens? I originally wanted to start with my favorite album, *Odyssey*, but it made more sense to begin with their latest single album, *Fame*.

I’m still very new to MIR, so this is more of a learning-by-doing exercise than a technical deep dive. I don’t have a music theory background, so most of this is just me trying to understand how the sound behaves over time using simple audio features.

Based on a few MIR books and resources, these are the basic features I explored:

- **Waveform + RMS** → overall loudness shape  
- **Mel spectrogram** → texture / brightness patterns  
- **Zero Crossing Rate** → how “busy” or sharp the sound is  
- **Spectral centroid** → timbral brightness  
- **Onset strength + beats** → rhythmic activity  
- **Chroma** → repeating pitch patterns (no theory needed; just visual shapes)  
- **Normalized overlay (RMS + ZCR + centroid)** → how these features move together  

---

## Feature Breakdown & What I Learned

### **Waveform + RMS Energy — Loudness & Structure**
The waveform is dense across the whole track, but the RMS plot makes the structure easy to see:
- A softer intro  
- A gradual build-up leading into each chorus  
- A consistent high-energy profile during the choruses  
- A sharp fall at the end  

Even with a compressed modern mix, RMS still reveals where the song expands or pulls back.

---

### **Normalized Timbre Features — RMS, ZCR, Spectral Centroid**
Overlaying these three features makes the shape of the song pop visually:
- **RMS** highlights overall energy  
- **ZCR** shows busy / percussive vocal moments  
- **Centroid** reflects brightness  

Together, they form a simple “fingerprint” of the track’s energy flow.

---

### **Mel Spectrogram — Texture & Frequency Shape**
The spectrogram shows:
- Strong, continuous low-frequency energy from the bass  
- Bright high-frequency accents in the chorus  
- Repeating mid-frequency patterns in the verses  
- Clear contrast between intro/verse vs. chorus  

It was satisfying to see how the song looks brighter and denser in the exact moments it *feels* brighter and denser.

---

### **Beat Markers & Tempo (143.6 BPM)**
The beat grid aligns tightly across the spectrogram, confirming:
- A steady tempo  
- Well-defined rhythmic structure  
- Strong alignment between beats and brightness spikes  

The track is rhythmically clean and consistent.

---

### **Onset Strength — “Impact Curve”**
The onset envelope shows:
- Frequent medium peaks → vocals + rhythmic hits  
- Tall spikes → transitions or strong percussive moments  
- Most activity in the chorus  
- Noticeable dips in calmer sections  

It basically visualizes “where the song hits.”

---

### **Chroma — Harmonic Activity Shapes**
Even without theory, the chroma features show:
- A repeating, loop-like harmonic structure  
- Brighter, more consistent columns during the chorus  
- More scattered patterns in the verses  

You can literally *see* the harmonic stability of the song.

---

## What I Took Away From This Project
This was my first attempt at MIR, so I didn’t try to be technically deep. I focused on:

- Learning how to read the plots  
- Understanding how audio behaves visually  
- Getting comfortable with basic features  
- Connecting visual patterns to how the music feels  

Fame as a song feels very full and busy to me, and the analysis aligned with that impression.

The full analysis was done in a Jupyter notebook.

---

## Full Notebook (Rendered below)
The complete code, plots, and experiments are included below.  
I’ll keep refining the notebook as I learn more about MIR.


<iframe 
    src="https://nbviewer.org/github/pubdomacc/mir-analysis-riize-fame/blob/main/notebooks/MIR-notebook.ipynb"
    width="100%" 
    height="900px"
    style="border:none;">
</iframe>

> If the embedded viewer does not load, click the link below to open it directly:
>
> 👉 **[https://nbviewer.org/github/pubdomacc/mir-analysis-riize-fame/blob/main/mir-fame/MIR-notebook.ipynb](https://nbviewer.org/github/pubdomacc/mir-analysis-riize-fame/blob/main/notebooks/MIR-notebook.ipynb)**

---


