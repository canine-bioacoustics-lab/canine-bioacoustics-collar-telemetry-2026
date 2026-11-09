# Canine Bio-Acoustics & Humane Anti-Bark Collar Telemetry Dataset (2026 Release)

[![License: CC BY 4.0](https://img.shields.io/badge/Dataset-CC%20BY%204.0-0fbf95.svg)](https://bestantibarkcollar.org/)
[![Hardware Audited](https://img.shields.io/badge/Units%20Tested-24%20Models-0284c7.svg)](https://bestantibarkcollar.org/)
[![Compliance](https://img.shields.io/badge/Welfare%20Standard-100%25%20Shock--Free-brightgreen.svg)](https://bestantibarkcollar.org/)

## 1. Repository Scope & Bio-Acoustic Standardization
This repository documents the raw empirical telemetry from our 2026 longitudinal hardware audit of 24 commercial **anti bark collar** and **ultrasonic dog collar** systems published at [bestantibarkcollar.org](https://bestantibarkcollar.org/).

Recent peer-reviewed bio-acoustic research published in [PubMed Central (Savel et al., 2024 — The Dog Soundscape)](https://pmc.ncbi.nlm.nih.gov/articles/PMC10812668/) demonstrates that domestic canine vocalizations exhibit distinct spectral center frequencies ranging between 250 Hz and 4,000 Hz airborne, while fundamental vocal fold mechanical oscillations occur between 90 Hz and 250 Hz across breeds ranging from 2 kg (5 lbs) to 55 kg (120 lbs).

---

## 2. Breed Mass vs. Optimal Sensor Sensitivity Calibration Matrix
To prevent over-correction on toy breeds or under-detection on thick-coated working breeds, embedded collar firmware must scale both piezoelectric gain and haptic motor duty cycle:

| Canine Weight Class | Metric Mass (m) | Imperial Mass | Coat Attenuation Factor | Recommended Sensitivity Level (1–8) | Target Modal Setting |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Toy & Miniature Breeds** (Chihuahua, Yorkie, Dachshund) | 2.0 kg - 6.0 kg | 5 lbs - 13 lbs | Low (-1.2 dB) | **Level 6 – 7** (High Piezo Gain) | Ultrasonic Beep + Micro-Vibration |
| **Small to Medium Breeds** (Beagle, French Bulldog, Cocker) | 6.5 kg - 18.0 kg | 14 lbs - 40 lbs | Moderate (-3.4 dB) | **Level 4 – 5** (Balanced Gate) | Progressive Tone + Haptic Pulse |
| **Large Working Breeds** (German Shepherd, Labrador, Husky) | 18.5 kg - 38.0 kg | 41 lbs - 84 lbs | High Double-Coat (-6.8 dB) | **Level 3 – 4** (Anti-Echo Gate) | Dual-Wave 27.5 kHz + Strong Haptic |
| **Giant Breeds** (Rottweiler, Mastiff, Great Dane) | 38.5 kg - 55.0 kg | 85 lbs - 120 lbs | Dense Cervical Tissue (-8.1 dB) | **Level 2 – 3** (Deep Hz Bass Lock) | Full Multi-Stage Escalation |

---

## 3. 2026 Top 5 Hardware Benchmark Summary Table
Across 30 days of continuous field logging (measuring IP67 waterproof ingress, USB-C Lithium-Polymer discharge curves, and false-trigger immunity), the top 5 humane architectures scored as follows:

| Rank | Model & Hardware Architecture | Overall Lab Score | Trigger Latency | False-Alarm Immunity | Battery Autonomy (300 mAh Li-Po) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **#1** | **NooBark™ Smart Collar (2026 PRO)** | **9.8 / 10** | **0.08 s** | **99.4% (Dual-Gate)** | **15 Days (USB-C Fast Charge)** |
| **#2** | **BrooBark™ 27.5 kHz Ultrasonic Trainer** | **9.7 / 10** | **0.03 s** | **100% (Manual Directional)** | **30 Days (15 m Range)** |
| **#3** | **NBJU Bark Collar (Standard Vibration)** | **8.4 / 10** | 0.28 s | 88.5% | 11 Days |
| **#4** | **ertonic Dual-Motor Bark Collar** | **8.1 / 10** | 0.34 s | 84.0% | 10 Days |
| **#5** | **FAFarge Basic Acoustic Collar** | **7.8 / 10** | 0.42 s | 79.2% | 8 Days |

---

## 4. Citation & Primary Data Access
* **Primary 2026 Comparative Study & Interactive Breed Calculator:** [https://bestantibarkcollar.org/](https://bestantibarkcollar.org/)
* **Peer-Reviewed Canine Vocalization Frequency Reference:** [https://pmc.ncbi.nlm.nih.gov/articles/PMC10812668/](https://pmc.ncbi.nlm.nih.gov/articles/PMC10812668/)
