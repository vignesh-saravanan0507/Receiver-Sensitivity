# Receiver-Sensitivity
# Optical Receiver Sensitivity Analysis

## Objective
Determine the sensitivity of a PIN photodiode-based optical receiver by calculating the minimum received power necessary to achieve a given Q factor. Compare simulation results with those obtained analytically.

---

## Theory
If only thermal noise is considered, the sensitivity of a PIN photodiode-based receiver is:



<img width="1126" height="718" alt="image" src="https://github.com/user-attachments/assets/22298a91-302d-41e4-b254-86c9b8ec704e" />

---

## Calculations
Receiver specifications:

| Parameter                        | Value                          |
|----------------------------------|--------------------------------|
| Operating bit rate               | 2.5 Gb/s                       |
| Bandwidth                        | 1.65 × bit rate                |
| Thermal noise spectral density    | X.Y × 10⁻²² A²/Hz              |
| Desired Q factor                 | 6                              |
| PIN photodiode responsivity      | 1 A/W                          |

> **Note:** X and Y are the last two digits of your student ID.  
> Example: If ID ends with **43**, then ST = 4.3 × 10⁻²² A²/Hz.  

Using the formulas above, calculate the receiver sensitivity.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f319f601-0746-42fa-a24f-a830880e7636" />
<img width="871" height="1280" alt="image" src="https://github.com/user-attachments/assets/69402af2-4441-4f0e-b267-3158818bbf91" />
<img width="1202" height="560" alt="image" src="https://github.com/user-attachments/assets/fd15a5c9-9705-423b-94fe-1d6a331e32fc" />

---

## Layout
The simulation layout consists of:
1. CW laser source  
2. NRZ modulator  
3. Optical attenuator  
4. PIN photodiode with electrical filter  

Settings:
- Responsivity = 1 A/W (default)  
- Dark current = 0  
- ASE noise = off  
- Thermal noise parameter = editable  

Power meters are placed:
- At the modulator output  
- After the attenuator (input to receiver)  

---

## Simulation
Steps:
1. Adjust output power to **0 dBm**.  
2. Set attenuator to **20 dB**.  
3. Run the simulation.  
4. Adjust attenuator until **Q factor = 6.00 ± 0.05**.  

---

## Report
Your report should include:
- Pre-lab calculations (attach handwritten work if applicable).  
- Screenshots or displays of simulation results:  
  - Power readings  
  - BER analyzer output  
  - Eye diagram  
- Discussion of differences between analytical and simulation results.  

---

## Result
Hence the output is successfully verified.
