# spectral-gate-releases

### Description
---
A frequency-independent gate. 

- The plugin uses the PFFFT library's FFT to derive 'bins' which represent individual frequencies on the spectrum. This plugin allows for FFT sizes between 256 blocks and 8192 blocks. 
- Each bin's magnitude is checked against the threshold and is either muted or let through, depending on the status of the invert parameter. 

### Features
---
- Selectable FFT size. Available sizes are 256, 512, 1024, 2048, 4096, and 8192.
- Input and output gain
- Invert. When enabled, bins whose magnitude is above the threshold are gated, while the bins with magnitudes below are let through.
- Threshold in DB
- A "curve" that allows the user to influence the behavior of the gate over different parts of the frequency spectrum
