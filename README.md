# 🎶 Five Band Audio Equalizer

## 📌 Introduction
An **audio equalizer** is a circuit that adjusts the output of different frequency bands within an audio signal. Equalizers are widely used in hi-fi systems to achieve superior sound quality across the audible spectrum.  

This project implements a **5-band analog audio equalizer** using operational amplifiers and transistors. After splitting the input signal into five distinct frequency ranges, the circuit applies adjustable gain to each band and displays the levels using sound indicators.

---

## Features

- **Five Frequency Bands:** Custom shaping for Bass, Low-Mid, Mid, High-Mid, and Treble ranges.
- **Analog Signal Path:** All audio processing is analog for true fidelity.
- **Visual Level Metering:** LM3915-based LED VU meter for monitoring output.
- **High-Quality Components:** Uses NE5532 op-amps for low noise and high slew rate.

---

## System Overview

- **Band 1:** Sallen-Key unity-gain low band
- **Bands 2–5:** Cascaded MFB band-pass filter stages
- **Amplification:** NE5532 op-amps in all stages
- **Level Display:** LM3915 IC driving a 10-segment LED bar graph

### Block Diagram

```
[Audio In] --> [Sallen-Key Low Band Filter] --> [MFB Band 2] --> [MFB Band 3] --> [MFB Band 4] --> [MFB Band 5] --> [Summing Amp] --> [Audio Out]
                                                  |
                                            [LM3915 LED Display]
```

---

## Bill of Materials (BOM)

| Component     | Quantity | Notes                                 |
|---------------|----------|---------------------------------------|
| NE5532 Op-Amp | Varied   | Main filter & amplifier stages        |
| LM3915        | 4        | LED VU meter                         |
| Resistors     | Varied   | See schematic                        |
| Capacitors    | Varied   | See schematic                        |
| Potentiometers| 6        | Band gain controls                    |
| LED Bars      | 4        | Output display                        |
| PCB/Perfboard | 4        | For circuit assembly                  |
| Audio Jacks   | 2        | Input/Output                          |
| Power Supply  | 1        | ±12V or as required by op-amps        |

---

## Schematics

See [`schematic.pdf`](schematic.pdf) or [`schematic.png`](schematic.png) (if present).
You can find the circuit diagram, filter specifications, and layout suggestions here.

---

## Assembly Instructions

1. Connect audio input and output jacks.
2. Double-check all connections for shorts and polarity.
3. Power up and test the circuit with a known audio source.

---

## Usage

- Adjust each potentiometer to boost/cut its associated frequency band.
- Monitor the output signal level using the LED display.
- Fine-tune filter frequencies and Q-factors by changing resistor/cap values (see schematic notes).

---

## Troubleshooting

- **No Output:** Check op-amp power pins, input/output jacks, and signal traces.
- **Distorted Sound:** Ensure proper supply voltage and correct filter component values.
- **LED Meter Not Working:** Verify LM3915 wiring and LED polarity.

---

## License

This project is licensed under the MIT License. See [`LICENSE`](LICENSE) for details.

---

## Contributing

Pull requests and suggestions are welcome! If you identify issues or want improvements, please open an issue or submit a PR.

---

## Author & Contact

Made by [SenudaHR](https://github.com/SenudaHR)  
For questions, contact via GitHub or open an issue.

---

## References

- Data Sheets: [NE5532](https://www.ti.com/lit/ds/symlink/ne5532.pdf) | [LM3915](https://www.ti.com/lit/ds/symlink/lm3915.pdf)
- Audio Equalizer theory: [Wikipedia](https://en.wikipedia.org/wiki/Equalization_(audio))
