# FLASHzero Documentation

## MRM2024: MR-zero meets FLASH

This repository contains sequence files and animations demonstrating the optimization process described in the article "MR-zero meets FLASH – Controlling the transient signal decay in gradient- and rf-spoiled gradient echo sequences."

### Data Files

RF phases for Task 2 are saved in the following files:
- `MRM2024/data/task2_rfphase_brain.npy`
- `MRM2024/data/task2_rfphase_phantom.npy`

### Task 2: RF Phase Details

#### Phantom
- **RF Phase File**: `task2_rfphase_phantom.npy`
- **Sequence Parameters**:
  - Flip Angle (α): 10°
  - Repetition Time (TR): 10 ms
  - Echo Time (TE): 5 ms
  - Readout Bandwidth: 217 Hz/pixel
  - Field of View (FOV): 200 mm
  - Slice Thickness: 10 mm
  - Matrix Size: 128 x 128
- **Tissue Properties**:
  - T1: ≈ 1.0 s
  - T2: ≈ 0.16 s
  - Relative B1 (rB1): ≈ 0.77
  - Diffusion Coefficient (D): ≈ 1.6 ∙ 10^(-3) mm²/s

#### Brain
- **RF Phase File**: `task2_rfphase_brain.npy`
- **Sequence Parameters**:
  - Flip Angle (α): 19.5°
  - Repetition Time (TR): 6 ms
  - Echo Time (TE): 3.2 ms
  - Readout Bandwidth: 500 Hz/pixel
  - Field of View (FOV): 200 mm
  - Slice Thickness: 10 mm
  - Matrix Size: 128 x 128
- **Tissue Properties**:
  - T1: ≈ 1.5 s
  - T2: ≈ 0.11 s
  - Relative B1 (rB1): ≈ 0.77
  - Diffusion Coefficient (D): ≈ 0.84 ∙ 10^(-3) mm²/s

### Colab MR-zero simulation
- You can run the Colab to simulate different standard rf increments or optimization tasks.
  - https://github.com/MRsources/FLASHzero/blob/main/MRM2024/FLASHzero.ipynb
  - https://colab.research.google.com/github/MRsources/FLASHzero/blob/main/MRM2024/FLASHzero.ipynb
- You can run the Colab to see the influence of the Epstein artifact on different sharp edges (Comparison with Gibbs Ringing)
  - https://github.com/MRsources/FLASHzero/blob/main/MRM2024/Epstein_Artifact_PSF.ipynb
  - https://colab.research.google.com/github/MRsources/FLASHzero/blob/main/MRM2024/Epstein_Artifact_PSF.ipynb
