# Temperament Visualizer

An interactive, self-contained musical temperament visualizer that demonstrates how different tuning systems divide the octave. Inspired by the Music Blocks Temperament Widget.

## What is Musical Temperament?
In music theory, a **temperament** is a tuning system that slightly compromises the pure intervals of just intonation to meet other musical requirements, such as the ability to play in multiple keys on a fixed-pitch instrument (like a piano).

- **12-TET (12-Tone Equal Temperament)**: The modern standard. It divides the octave into 12 equal logarithmic steps. While versatile, it makes every interval (except the octave) slightly "out of tune" compared to natural harmonic ratios.
- **EDO (Equal Division of the Octave)**: Systems like 19-EDO or 31-EDO divide the octave into more steps, often achieving closer approximations to pure intervals than 12-TET.
- **Just Intonation**: Tuning based on whole-number ratios (e.g., 3:2 for a perfect fifth). It sounds "pure" but is difficult to use when modulating between keys.

## How to use this Visualizer
1. **Circle of Notes**: Each dot represents a note in the selected temperament. The angle corresponds to the pitch (0 to 360 degrees = one octave).
2. **Comparison Mode**: Toggle "Compare with 12-TET" to see how the chosen temperament deviates from the modern standard.
3. **Measure Intervals**: Click any two notes to see the mathematical ratio and cents deviation between them.
4. **Frequency Table**: View precise Hertz values and cents deviation relative to the nearest 12-TET note.

## Technical Details
- **Core Math**: 
  - EDO Angle: `360 * step / N`
  - Ratio Angle: `360 * log2(ratio)`
  - Cents: `1200 * log2(freq / base)`
- **Technology**: Vanilla HTML5, CSS3, and Canvas API. No external libraries required.

## Relation to Music Blocks
This tool follows the same logic used in the **Music Blocks Temperament system**, allowing students and musicians to visualize the "geometry of sound" and understand why certain tuning systems sound more "consonant" or "dissonant" than others.
