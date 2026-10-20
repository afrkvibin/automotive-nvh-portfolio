# Week 1 – Signal Basics

## Frequency
The number of cycles or repetitions per unit time. It's measured in hertz (Hz), where 1 Hz is one cycle per second. The period is the time for one cycle: T = 1/f.

## Amplitude
The maximum displacement of the wave away from its equilibrium.

## Phase
An angle-like measure that tells you the position of a wave in its cycle.

## Sampling rate
A sample is the value of a signal at a point in time or space. The sampling rate is the number of samples taken per second, in Hz. For example, at 1000 Hz you take 1000 samples every second.

## Time-domain signal
A representation of how a signal or quantity varies with time.

## Why sample at more than 2× the highest frequency?
The Nyquist–Shannon sampling theorem gives the minimum sampling rate needed to reconstruct a continuous-time analog signal without losing information. That minimum is more than twice the highest frequency in the signal.

If you sample too slowly, a high frequency shows up as a false lower frequency. This is called aliasing, like wagon wheels that seem to spin backwards in films. Aliasing can't be undone after recording, so in NVH you set the sampling rate above twice the highest frequency you care about.