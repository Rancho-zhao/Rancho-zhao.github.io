---
title: "A Design of Audio Amplifer"
collection: projects
type: "Projects"
permalink: /projects/2019-06-11-project-audio
date: 2019-06-11
---

I designed a audio amplifer that includes four functions: microphone amplification, volume control, mixing function and adjustable tone.

The performance indicators of this amplifier are:

| Items | Information |
| ------| ----------- |
| Rated power| $\ge 0.5W(THD\le10\%)$ |
| Load impedance| $10\Omega$|
| Frequency response| $f_L\le 50Hz$,$ f_H \ge 20kHz$|
| Input impedance| $\ge 20k\Omega$|
| Voice input sensitivity| $\le 5mV$|
| Tone control characteristics| $0dB$ gain at 1kHz, $\pm 12dB$ adjustment range at $125Hz$ and $8kHz$|

## Voice amplifier
I use a phase amplifier: $U_o=(1+\frac{R_3}{R_2})U_i$, $R_3 = 100k\Omega$, $R2 = 20k \Omega$, $A_u=6$. The capacitors are used for filtering.

![fig1](/images/project-audio/voice.jpg "voice amplifier")

## Mixing amplifier
The function of a mixing amplifier is to mix and amplify voice signals and music signals, as shown in the circuit diagram blow. It can be seen that the relationship between output voltage and input voltage is $U_o=-(\frac{R_3}{R_4} * U_{i1}+\frac{R_3}{R_5} * U_{i2})$. The gain can be adjusted by adjusting the potentiometer.

![fig2](/images/project-audio/mix.jpg "mixing amplifier")

## Power amplifier
The power amplifier circuit is implemented using LM386, with an amplification factor of approximately 20 times.

![fig3](/images/project-audio/power.jpg "power amplifier")

## Tone control circuit
The function of tone control is to control and adjust the output frequency of the audio amplifier, and the control curve is shown by the line in the figure. As shown in the figure, the tone controller only improves or attenuates the gain at low and high frequencies, while the gain at intermediate frequencies remains unchanged. So the circuit of the tone controller consists of a low-pass filter and a high-pass filter.

![fig4](/images/project-audio/control-1.jpg "Tone control circuit")

![fig5](/images/project-audio/control-2.jpg "Tone control curve")