# A Replicable Open‑Source Wearable System for Human‑Centric Light Research  
**Integrated hardware and software for spectral acquisition and multi‑metric assessment of visual and non‑visual light effects**

## Research Questions

This project investigates whether a **low‑cost, open‑source wearable spectroradiometer** can reliably measure **visual** and **non‑visual** effects of light in everyday environments. Specifically:

1. **How does the accuracy of a DIY/DIT spectroradiometer compare with professional commercial instruments?**  
2. **Is measurement performance affected by long‑term use, the 3D‑printed housing, or auxiliary sensors integrated on the same MCU?**  
3. **Do visual and non‑visual metrics (e.g., photopic illuminance, melanopic EDI) computed through Python scripts differ from those produced by commercial software tools or CIE S 026 Toolbox?**

## Our Approach

We developed an **open‑source wearable device** incorporating:

- A **nanolambda nSP32m** compact spectroradiometer  
- A **Raspberry Pi** microcomputer  
- Additional environmental sensors  
- A **custom 3D‑printed wearable enclosure**  
- A fully transparent **Python analysis workflow** using LuxPy and CIE S 026:2018 methods

Two measurement campaigns validated the prototype:

### **1. ZEB Lab (ITC‑CNR, San Giuliano Milanese)**  
- Compared low‑cost spectroradiometers, the **nanolambda NSP32m (LC1‑sp)** and the **nanolambda XL500 (LC2‑sp)** with **DeltaOhm HD30.1 + HD30.S1 (PR1‑sp)**  
- Tested LED, halogen, fluorescent, incandescent, and daylight sources  
- Illuminance range: **50–500 lx**, CCT: **2500–7000 K**

### **2. SENS i‑Lab (University of Campania "Luigi Vanvitelli")**  
- Compared the wearable configuration with **Konica‑Minolta CL‑70F (PR2‑sp)**  
- Evaluated:  
  - Possible performance degradation over time  
  - Optical distortion due to enclosure geometry  
  - Interference from other onboard sensors  
- Low illuminance scenarios (**15–45 lx**) to assess sensitivity and noise levels  

## First Results

- **LC1‑sp** accurately reproduces spectral trends of the reference devices (PR1‑sp and PR2‑sp).  
- **LC2‑sp** shows errors when the sensing element is partially shaded, emphasizing correct sensor placement.  
- No measurable **time degradation**, **housing‑induced distortion**, or **multi‑sensor interference** was observed.  
- **Python‑based LuxPy + CIE calculations** match proprietary software results (R² ≈ 1).  
- The device is reliable for **continuous, wearable, real‑world monitoring**, overcoming limitations of traditional spectroradiometers that require fixed positioning, manual acquisition, and controlled conditions.

The methodology and results are presented in:

**A Replicable Open‑Source Wearable System for Human‑Centric Light Research**  
F. Salamone, G. Ciampi, M. Scorpio, M. Masullo, L. Danza, M. Ghellere,  
A. Devitofrancesco, A. Bellazzi, S. Sibilio.  
(Full reference/DOI will be added upon publication.)

If you use this repository, please cite the related article (DOI forthcoming)  
along with this repository.

## Why Open Source?

Professional-grade spectroradiometers are accurate but not suitable for:

- long-term monitoring  
- mobility or wearable use  
- large-scale data collection  
- unobtrusive daily-life studies  

#### Example video illustrating the PR1‑SP acquisition steps (click on the image below, and remember that the video has been sped up by a factor of 10):
[<img width="301" height="407" alt="image" src="https://github.com/user-attachments/assets/2eaba38f-78f6-4265-b4fb-33ce61648eba" />](https://youtube.com/shorts/vFOOwzJvH8o?si=PPmpHsuS9cYaFXWf)

This open-source system enables:

- **Reliable, autonomous spectral monitoring**  
- **On-device computation of visual and non-visual metrics**  
- **Affordable scaling for population studies**  
- **Fully transparent, reproducible workflows**

#### Example video showing the LC1‑SP automatic acquisition approach (click on the image below, and remember that the video has not been sped up):
[<img width="581" height="262" alt="image" src="https://github.com/user-attachments/assets/b35c8d8e-4b1c-4fec-a9ba-c517c6e0b607" />](https://www.youtube.com/watch?v=3A9F1TD3kME?si=_e-iThfWU_JiZLf4)

Our goal is to make human‑centric light monitoring **accessible, modifiable, and scientifically robust**.

## Repository Contents

(To be updated with actual links)

- 3D‑printed enclosure and mounting files  
- Firmware and acquisition scripts  
- Python pipelines implementing LuxPy and CIE S 026 metrics  
- Measurement datasets and comparison plots  
- Calibration procedures and documentation  

## Author Contributions

- **Francesco Salamone** – Conceptualization, Methodology, Hardware and Software design and development, Data curation, Validation, Visualization, Writing – original draft, Writing – review & editing  
- **Giovanni Ciampi, Michelangelo Scorpio** – Data curation for PR2-sp on the SENS i-lab test, Writing – review & editing  
- **Massimiliano Masullo** – Supervision, Conceptualization, Methodology, Writing – review & editing  
- **Ludovico Danza** – Funding acquisition for spectroradiometer modules, Writing – review & editing 
- **Matteo Ghellere, A. Devitofrancesco, A. Bellazzi** – Data curation for PR1-sp on the ZEB lab test, Writing – review & editing
- **Sergio Sibilio** – Supervision, Conceptualization, Methodology, Validation, Writing – review & editing  

## License  
### CC Attribution‑NonCommercial 4.0 International

This work is licensed under a  
[Creative Commons Attribution‑NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/)

[![CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc/4.0/)
