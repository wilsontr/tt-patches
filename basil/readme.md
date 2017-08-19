# Basil

Basil is a Pure Date patch comprising a dual oscillator intended for use on mxmxmx's Terminal Tedium Eurorack module. The oscillators (VCOs) can be shaped from sine to sawtooth, cross-modulated, mixed together, ring-modulated, and run through a wavefolder. VCO 2 can be used to reset the phase (sync) VCO 1, and both VCOs can be synced to outside audio sources. 

This algorithm is based on the phase-modulation mode in [Noise Engineering's Loquelic Iteritas](https://www.noiseengineering.us/loquelic-iteritas/) Eurorack module. 

This is not a clean algorithm. There is no oversampling, so things can get dirty and nasty quickly. But that's the point. 

## Controls

![Controls](https://raw.githubusercontent.com/wilsontr/tt-patches/master/basil/basil-layout.png)

### Pitch

Controls the pitch of each oscillator.

### Waveshape

Fades the waveshape of both oscillators from sine to sawtooth.

### Crossmod

Phase-modulates each oscillator by the other in a feedback configuration. 

### Mix

Fades the Mix output from VCO 1, to the ring modulated product of VCO 1 and 2, to VCO 2. 

### Wavefolder

Adjusts the amount of wavefolding on the resulting mixture.

### Sync On

Causes VCO 1's waveform to be reset by VCO 2. This can generate many additional harmonics.

### Sync In 1/2

Allows VCO 1 and 2 to be phase-reset by external audio sources.

### Mix Out

The output of the wavefolder stage is sent here.

### VCO 2 Out 

The output of VCO 2 before the Mix crossfader is sent here.