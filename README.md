# 🎶 Five Band Audio Equalizer

## 📌 Introduction
An **audio equalizer** is a circuit that adjusts the output of different frequency bands within an audio signal. Equalizers are widely used in hi-fi systems to achieve superior sound quality across the audible spectrum.  

This project implements a **5-band analog audio equalizer** using operational amplifiers and transistors. After splitting the input signal into five distinct frequency ranges, the circuit applies adjustable gain to each band and displays the levels using sound indicators.

---

## 📐 Specifications

- ✅ **Five Adjustable Frequency Bands**
  - **20 Hz – 300 Hz** (Bass)
  - **300 Hz – 1 kHz** (Low Midrange)
  - **1 kHz – 4 kHz** (Midrange)
  - **4 kHz – 10 kHz** (Upper Midrange)
  - **10 kHz – 20 kHz** (Treble)

- ✅ **Analog Electronics Implementation**
  - Transistors and Operational Amplifiers (Op-Amps)
  - Active band-pass filters per frequency range

- ✅ **Features**
  - Independent gain control for each frequency band  
  - Protection against **signal saturation/clipping**  
  - **Audio level indicators** for visual feedback per band  
  - Input interface for external audio devices  
  - Housed in a robust and aesthetic **enclosure**

---

---

## ⚙️ Implementation Details
- **Band Separation**: Achieved using band-pass filter circuits designed with Op-Amps.  
- **Gain Adjustment**: Each band has a variable resistor (potentiometer) for tuning gain.  
- **Signal Integrity**: Additional circuitry ensures no unwanted distortion or saturation.  
- **Indicators**: LED or VU-meter style displays represent the amplitude of each band.  
- **Enclosure**: Custom housing ensures durability and usability.  

---

## 🚀 Usage
1. Connect an **audio input** (phone, laptop, player, etc.) to the input jack.  
2. Adjust the **gain knobs** for each of the 5 bands.  
3. Observe **band level indicators** to monitor output per frequency range.  
4. The processed signal is available at the **output jack** for speakers/amplifiers.  

---

