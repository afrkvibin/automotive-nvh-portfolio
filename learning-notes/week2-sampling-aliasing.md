# Week 2 – Sampling & Aliasing

Demo notebook: [week2-aliasing-demo.ipynb](week2-aliasing-demo.ipynb)


## Sampling rate and Nyquist
Sampling rate is the number of times you take a sample of a signal per second.

You have to sample your signal at a rate at 2 times the highest frequency of the original signla so as to not lose information. That is basically the Nyquist theorem Fs>2Fmax


## Aliasing

Aliasing basically is when you don't follow the Nyquist theorem so the reconstructed signal ends up having low frequency components that were not present in the original..


## Units
- Hz: Measures frequency—the number of complete cycles, waves, or oscillations that occur in one second.
- rad/s: Measures angular velocity—how fast an object rotates or how quickly an angle changes per second.
- s: The SI base unit of time.
- Pa: Measures pressure or stress—the amount of force applied uniformly over an area
- m/s²: Measures acceleration—the rate at which an object's velocity changes over time.
so that the continuous time analog signal can be reconstructed without information loss
Frequency-number a cycles or repetitions per unit time

amplitude - maximum displacement of the wave away from its equilibrium

pahse - and angle like measure that will tell you the position of a wave in its cycle

sample - is the value of a signal at a point in time or space

Nyquist–Shannon sampling theorem - defines the minimal sampling rate needed in order to reconstruct a continuous time analog signal

Time-domain signal is a representation of how a signal or quantity varies with time

## Why sample at more than 2× the highest frequency?
so that the continuous time analog signal can be reconstructed without information loss
## Solved examples
**Example 1:** 700 Hz tone sampled at fs = 1000 Hz.
- Nyquist frequency = fs / 2 = 500 Hz
- Alias = |f − k·fs| = 300 Hz
- Checked in Python (week1-sine-wave.ipynb, last cell): 300
