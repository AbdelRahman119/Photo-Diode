# Photo_Detector

## Introduction

- This VerilogA module, named "Photo_Detector," models the behavior of a photodiode in response to incident optical power. The module calculates the photocurrent generated by the photodiode based on the input electric field magnitude and phase.
- The photo detectors are reverse biased diodes which produce currents that are proportional to the power of light falling on Them (I_PD=R*P) where R is the responsivity of the photodiode and since the power of the light is proportional to square its electric field so, PDs behave as mixers that mixes Es with ELO.
- The model also, includes the shot shot noise generated by the Photo Diode.
## Module Inputs and Outputs

- **Inputs:**
  - E_real: Real component of the incident electric field.
  - E_img: Imaginary component of the incident electric field.

- **Outputs:**
  - iout_p: Photocurrent output from the photodiode (positive terminal).
  - iout_n: Photocurrent output from the photodiode (negative terminal).

## Parameters

- **Responsitivity:** Responsitivity of the photodiode, indicating its sensitivity to incident optical power.
- **cap:** Capacitance of the photodiode.
- **Rs:** Series resistance of the photodiode.

## Analog Behavior

The module includes an analog block where the photocurrent is calculated based on the square of the magnitude of the incident electric field and the responsivity of the photodiode.

## Usage

1. **Input Parameters:** Provide the input parameters E_real and E_img to the module.
2. **Simulation:** Simulate the VerilogA module using a compatible simulator, ensuring proper connection of input and output ports.
3. **Observation:** Analyze the output signals iout_p and iout_n to understand the photocurrent generated by the photodiode.
