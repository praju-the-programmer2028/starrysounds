# 🌌 Starry Sounds

## My Work

**Video:** https://youtu.be/imSuz52wqSE  
**Website:** https://praju-the-programmer2028.github.io/starrysounds/  
**Code:** https://github.com/praju-the-programmer2028/starrysounds  

---

## Description

Starry Sounds is an interactive web interface designed to introduce simple night instrumentals to curious listeners, whether it’s sitting in the grass under a starry sky or taking night strolls.

The experience unfolds like an animated storybook. The viewer flips through a hand-drawn nighttime picture book accompanied by gentle ambient music until the scene transitions into a sound menu. To hear the instrumentals, users tap sound panels.

The project combines audio, visual, and sensory cues. It is designed as an immersive gift-like experience that allows users to emotionally connect with traditional instrumental tones.

---

## Background

Growing up, I tried multiple instruments such as guitar, ukulele, drums, viola, and also completed basic Carnatic music training. None of the formal music theory fully stuck with me, but the experience of listening and practicing stayed.

That shaped how I hear rhythm today. I notice beats, staccatos, falsettos, and subtle shifts in sound that can completely change my mood.

Out of all the instruments I explored, harmonica and xylophone resonated the most with me. They are accessible, welcoming, portable, and versatile. They can also produce a wide range of melodies. For my first woodworking workshop in middle school, I built those instruments.

I also experimented with music mixing in GarageBand and uploaded tracks to SoundCloud. Even though the results were not studio perfect, they showed me something important. Creating melodic sound can be simple and personal.

The idea of combining simple melodies shaped the foundation of Starry Sounds. I built the experience around homemade and traditional instruments to promote cultural appreciation.

This was also inspired by moments with friends sharing different languages and music styles including K-Pop, Malayalam, Tamil, Bollywood, Hip-hop, Jazz, Pop, and Chinese classics. These small moments of connection feel especially meaningful in a calm, starry night setting.

I also wanted to include an experience that could resonate with people who experience synesthesia, where audio, visual, and sensory cues blend together.

---

## Setting The Stage

### Narrative Design

Every visual in the project is hand-drawn using Krita with a consistent palette:

- Dark navy background: #2B3D50  
- Cream or white outlines: #E8DFD0  
- Gold highlights for text: #E8A820  

To create animated transitions, I used CSS animations and transitions including fades, particles, and ripple effects, along with vanilla JavaScript sequencing and interaction.

Similar to music videos or Pixar-style storytelling, I designed the experience to begin with a narrative before introducing sound interaction.

---

### Scenery Into the Night (Slides 1–9)

Storybook-style transition into a nighttime environment.

---

### Introducing Tool Name

A pop-up appears after music notes are introduced.

---

### Music Notes Follow (Slides 10–13)

Transition from storytelling into interactive sound mode.

---

## Sound Design

Instead of using pre-recorded audio files, I used an open-source sound synthesis system.

### Narrative Ambient System

- Pentatonic night scale: A, C, D, E, G  
- Notes scheduled using AudioContext clock  
- A low A drone plays throughout the story and turns off at the brand reveal  

---

### Instrument Sound Groups

**Group 0 (Xylophone, Maracas, Wind Chimes)**  
Bright percussive tones using triangle waves (A5–C#6–E6), creating mallet and chime-like textures.

**Group 1 (Flute, Erhu, Pipa)**  
Breathy sine-based tones with a 5Hz vibrato LFO, creating wind-like expressive sound.

**Group 2 (Wooden Drums, Harmonica, Bell)**  
Harmonic tones using partials [1, 2.76, 5.4, 8.93] with exponential shaping.

---

## Instrument Design Mapping

Each instrument was intentionally designed to connect structure with sound:

- Xylophone: vertical wooden bars of varying length  
- Maracas: egg-shaped handheld shakers  
- Wind Chimes: hanging metal or wood tubes tied like a mooncatcher  
- Flute: cylindrical tube with finger holes  
- Erhu: thin stick with a resonating body  
- Pipa: oblong lute with vertical strings  
- Wooden Drums: wooden shells with sticks and cloth tension  
- Harmonica: rectangular body with air channels  
- Bell: trapezoidal bell shape with inner clapper  

I used Claude Code to help identify and match instrument note structures, especially for pipa, wind chimes, and erhu.

Images were embedded using HTML5 Base64 encoding as clickable panels.


After implementation, these became clickable sound panels for interaction.

---

## Final Implementation Notes

I wanted to create a chalkboard-like aesthetic with a raw and organic immersive feel using a consistent style including Caveat font and a navy, cream, and gold palette.

Even though I forgot much of my early music theory, I revisited simple instrumental tones and categorized them into groups. Building this at 19 felt like reconnecting with something I struggled to understand at 9.

Key features include:
- Click-to-advance story slides  
- Animated pop-ups and waveform visuals  
- Base64 image embedding  
- Clickable sound panels  
- Fade transitions and synchronized audio and visuals  

---

## Challenges

- Claude Code initially cropped instrument layouts unevenly  
- Some images were misaligned or mislabeled  
- Manual fixes were needed for spacing and panel structure  
- Base64 embedding (about 2.3MB total) required debugging for loading stability  
- Layout responsiveness issues where the storybook displays best on smaller screens  
- Back navigation bug in the second instrument slide  

---

## Future Improvements

- Recording feature with export to mp3, wav, or mp4  
- Volume sliders per instrument  
- Expanded instrument database  
- Multiple tones per instrument or sound switching system  
- Community sharing via SoundCloud, GarageBand, or YouTube  
- User accounts for saving and uploading sound creations  

---

## Reflection

This project helped me realize the value of my digital musical piece. I stepped out of my comfort zone by hardcoding every part.

The real learning came from exploring cultural instrumental tones and translating them into structured sound systems.

Different reactions from users included:
- Erhu and flute made people laugh  
- Harmonica and drums created a quiet reflective mood  
- Wind chimes and maracas created excitement and engagement  

At the end, the sounds felt simple, expressive, and human. The project is about listening, feeling sound, and creating emotional connections through simple melodies.

It recreates moments where sound drifts softly and combines into something immersive that can be experienced anytime with a click.

---

## References

- Base64 images in HTML: https://developer.mozilla.org/docs/Web/HTML/Element/img  
- CSS Animations: https://developer.mozilla.org/docs/Web/CSS/CSS_Animations  
- requestAnimationFrame: https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame  
- CSS Transitions: https://developer.mozilla.org/en-US/docs/Web/CSS/transition  
- Event Listeners: https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener  
- Web Audio API: https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API/Using_Web_Audio_API  
- Web Audio Guide: https://web.dev/articles/webaudio-intro  
- MDN Audio Examples: https://github.com/mdn/webaudio-examples  
- Touch Events: https://developer.mozilla.org/docs/Web/API/Touch_events  
- DOM: https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model  
