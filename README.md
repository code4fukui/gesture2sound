# gesture2sound

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A web-based synthesizer that transforms touch, pen, and mouse gestures into sound.

## Demo

**[https://code4fukui.github.io/gesture2sound/](https://code4fukui.github.io/gesture2sound/)**


![gesture2sound demo showing multi-touch interaction with anchor points and moving heads creating sound](https://user-images.githubusercontent.com/1552847/235282798-299f2203-9069-42b3-9602-5509e530058b.gif)


## Concept

This application works like a virtual string instrument. When you touch the screen, you create an **anchor point**. As you drag your finger or mouse away from this anchor, you "pull a string," generating a sound. The direction and distance of your pull, along with the pressure of your touch, dynamically shape the note's pitch, volume, and timbre.

## Features

-   **Expressive Control:** Dynamically modulate sound using the position, distance, and pressure of your input.
-   **Multi-Touch/Pen Support:** Play multiple notes simultaneously to create chords and complex soundscapes.
-   **Intuitive Visual Feedback:** Each input is represented by an anchor point and a moving "head," clearly showing how your gesture maps to the sound.
-   **Real-time Sound Synthesis:** Utilizes the Web Audio API to morph waveforms in real-time, from a pure sine wave to a rich, harmonic tone.

## How to Play

1.  **Start the Engine:** Click the **Audio ON** button to enable the Web Audio context (a browser requirement).
2.  **Create a Note:** Press and hold on the screen with your finger, mouse, or pen. This sets an **anchor point**.
3.  **Shape the Sound:** Drag away from the anchor point to begin playing and modulating the note.

### Controls

-   **Pitch (Frequency):** Controlled by the **horizontal distance** from the anchor. Move right for higher pitches, left for lower pitches. The scale is logarithmic, corresponding to musical octaves.
-   **Volume (Gain):** Controlled by the **vertical distance** from the anchor. Move up for louder volume, down for softer volume.
-   **Timbre (Harmonics):** Controlled by **pressure**. Lighter pressure creates a pure sine wave, while firmer pressure adds odd harmonics, morphing the sound towards a square wave.

## License

MIT License — see [LICENSE](LICENSE).