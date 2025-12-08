# FAME - a MIR Analysis

This project started out of my interest in Music Information Retrieval and, of course, my love for RIIZE’s music. So I figure, why not look at their tracks through MIR lens? I was going to start the exploration with my favorite album to date, Odyssey, but I think it made more sense to begin with latest single album, Fame. 
I'm still very new to MIR, so this project is totally a learning-by-doing type of exercise rather than a technical deep dive. I don't have a music theory basis, so it's just mosly me trying to understand how the sound behaves over time.

Based on the few MIR literature book, there are simple feature in audio data : loudness, brightness, noisiness and rhytmic events.

Said features are : 
- Waveform + RMS → overall loudness shape
- Mel spectrogram → texture / brightness patterns
- Zero Crossing Rate → how “busy” or sharp the sound is
- Spectral centroid → brightness
- Onset strength + beats → rhythmic activity
- Chroma → repeating pitch patterns (no theory needed; just shapes)
- Normalized overlay (RMS + ZCR + centroid) → how these features move together


## What I Took Away From This Project

This was my first attempt at MIR, so I didn’t try to be technically deep.
I focused on:

Learning how to read the plots
Understanding how audio behaves visually
Getting comfortable with basic signal features
Connecting visual patterns to how the music feels
The analysis was done in a Jupyter notebook.  

Fame as a song feels very noisy and full to me. So with all of the audio analysis done in the previous point this was aligned with what I feel.

## Full Notebook (Rendered below)
The complete code, plots, and experiments are included here.
I’ll keep refining the notebook as I get more comfortable with MIR concepts.

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


