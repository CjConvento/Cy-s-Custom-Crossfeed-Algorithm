# 30° Stereo Crossfeed & Modular Parametric EQ Suite

A custom crossfeed algorithm script designed to mimic speaker's exact delay of 0.32ms and eliminate the artificial "in-your-head" stereo isolation blob inherent to standard iem and headphones.

## Repository Contents

### 1. 30° Crossfeed Engine (`crossfeed-30deg.txt / crossfeed-30deg.jsfx)
A spatial processing script that simulates a **30-degree studio monitor environment** by cross-feeding audio signals with precise temporal delay and head-shadowing attenuation.
*   **Interaural Time Delay (ITD):** 0.32 ms (~15 samples at 48kHz)
*   **Head-Shadowing Simulation:** High-Shelf Filter (Fc = 1200 Hz, Gain = -6 dB, Q = 0.5)
*   **Acoustic Mix:** 75% Native Signal / 25% Filtered Crossfeed Signal

## Platform Compatibility & Routing Pipeline

This script is customizable and structured to be stacked sequentially in your audio pipeline (Load Crossfeed Engine ➔ Adjust to taste).

*   **Windows Desktop:** Compatible with **Equalizer APO** via declarative configuration lines.
*   **Android Mobile:** Fully supported via **JamesDSP** (utilizing the native Live Programmable JSFX engine for Crossfeed) and **ViPER4Android**.

## Setup Instructions

1.  **For Crossfeed Processing:** Download the script file and load it natively into Equalizer APO as included file(`crossfeed-30deg.txt`) or the (`crossfeed-30deg.jsfx`) for JamesDSP/Viper4Android Programmable DSP module.
