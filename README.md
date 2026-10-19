#Bell-State-Encoded Meta-Holography: PRQST Data
This repository contains the experimental count maps used for pixel-resolved quantum-state tomography (PRQST) in the study “Bell-State-Encoded Meta-Holography.”

Data acquisition
Two-photon coincidence images were acquired for 16 joint polarization-projection settings, using horizontal (H), vertical (V), diagonal (D), and left-circular (L) polarization projections in each photon arm.
For each projection setting, 10,000 camera frames were summed pixel by pixel and the resulting accumulated count map was saved as a plain-text (.txt) file. Each TXT file therefore represents a frame-summed, spatially resolved count image.

File naming and background measurements
For each polarization-projection setting, two corresponding TXT files are provided:
Without the bg suffix (for example, 1HhHs.txt): the shutter in photon arm b was open. The accumulated count map contains signal and background contributions.
With the bg suffix (for example, 1HhHsbg.txt): the shutter in photon arm b was closed to block the signal photons. The accumulated count map represents the background measurement.
For background acquisitions, the pump laser, herald detection, and camera acquisition settings were kept unchanged. The saved TXT files contain the accumulated measurements before background subtraction and quantum-state reconstruction.

Data analysis
The background maps and signal-plus-background maps are used to obtain background-corrected coincidence measurements for each polarization projection. Pixel-resolved two-photon polarization density matrices are then reconstructed from the 16 projection settings, as described in the manuscript's Materials and Methods section. The background modeling, quantum-state reconstruction, and uncertainty-estimation procedures are described there and in the Supplementary Materials.
