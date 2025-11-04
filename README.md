# 65nm NMOS Transistor Simulation using SILVACO TCAD

---

## 📄 Overview

This project presents a **simulation study of 65nm NMOS transistors** using **SILVACO TCAD (Athena & Atlas)**.
It reproduces the process and structure described in a reference paper, and compares the electrical characteristics of conventional 65nm NMOS, Halo-implanted, and Retrograde Well structures.

---

## 📁 Project Structure

```
├── FINAL_300nm.in
├── FINAL_65nm.in
├── FINAL_65nm_halo.in
├── *.set        # tonyplot setting files
├── *.log        # simulation output logs
├── *.str        # structure files
```

---

## ⚙️ Simulation Description

### 1. Baseline Comparison

* **300nm NMOS vs 65nm NMOS**
* Analysis of drain current variation by gate length
* ID–VD and ID–VG plots under different bias conditions

<img width="2452" height="1414" alt="image" src="https://github.com/user-attachments/assets/1c40287e-2b61-4a5e-b8b0-c621d12ce082" />


---

### 2. Halo & Retrograde Well Effects

* Comparison between conventional 65nm, Halo-implanted, and Retrograde Well NMOS
* Verification of short-channel effect (SCE) suppression
* Improvements in threshold voltage, saturation behavior, and leakage reduction
  
<img width="2478" height="1424" alt="image" src="https://github.com/user-attachments/assets/9c323db8-b532-4c40-833c-f5903bddb168" />

---

## 📊 Theoretical Background

* **Short Channel Effect (SCE):**
  As the channel length scales down, the drain electric field extends into the channel, weakening gate control and increasing leakage current.

* **Channel Length Modulation (CLM):**
  In saturation, drain current increases with drain voltage due to channel shortening near the drain.

* **Halo Implantation:**
  Locally doped regions near source/drain mitigate DIBL and stabilize the channel potential.

* **Retrograde Well:**
  A vertical doping profile with higher concentration deep in the substrate prevents punch-through and enhances output resistance.

---

## 🔍 Results Summary

* Simulated curves show strong qualitative agreement with the reference paper.
* Quantitative differences are due to unspecified sweep conditions (Vd/Vg) and slightly lower doping doses.
* Halo and Retrograde Well structures demonstrated:

  * **Increased threshold voltage**
  * **Improved current saturation**
  * **Reduced leakage current**

300nm
<img width="2430" height="1416" alt="image" src="https://github.com/user-attachments/assets/bf9b6d3e-a244-48ca-9194-ffb94c6e6ea9" />


65nm
<img width="2420" height="1424" alt="image" src="https://github.com/user-attachments/assets/afd50b3b-f1d5-448c-b463-110581ef9ffa" />



---

## 🧠 Notes

* The project is for **academic and research purposes**, and results may differ from real semiconductor fabrication.
* When editing `.in` files, be careful with **mesh definitions** and **implant dose/energy** parameters.
* Simulations were conducted using **Athena for process** and **Atlas for device characteristics**.

---
