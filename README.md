# 🧪 Thermo-Calc Simulation Reports — Summary Documentation

Author: **Siriro, Wiseman**  
ID: **S333263**  
Affiliation: **Polytechnic University of Turin — Italy**

---

## 🧷 Report 1 — Al–Sc Alloy Precipitation (DICTRA)

### 🎯 **Objective**
Simulate precipitation of **Al₃Sc** particles in **Al–0.3 wt% Sc** alloy under:
- Cooling from **650°C → 400°C** at **5 K/s**
- **Isothermal hold:** 1 hour @ 400°C
- **Geometry:** Spherical
- **Width:** 2 μm
- Outputs:
  - Total phase fraction of Al₃Sc vs time
  - Interface position vs time

---

### ⚙️ **Method Summary**
| Step | Description |
|---|---|
| System Definer | Selected *Demo Aluminum–based alloys*; elements: Al, Sc |
| Initial Equilibrium | Initial phase identified as **FCC_A1#1** at 650°C |
| Numerical Model | DICTRA diffusion demo with spherical geometry |
| Thermal Profile | Non-isothermal → Isothermal |

---

### 📉 **Key Observations**
#### **Phase Fraction Evolution**
- Rapid initial rise due to predefined precipitates
- Continued growth during diffusion phase
- Growth slows during long isothermal stage

#### **Interface Position**
- Fast nucleation stage: interface grows from **0 → ~0.020 μm**
- Slower diffusion-limited growth: reaches **~0.042 μm**
- Minimal change afterward during 3600 s holding

---

### 🧠 **Interpretation**
Cooling reduces Sc solubility in Al, promoting precipitation:
> ↓ Temperature → ↓ Solubility → ↑ Precipitation of Al₃Sc

Early stage dominated by nucleation & growth; later stage by diffusion limitations.

---

## 🧷 Report 2 — Cementite Precipitation in Steel

### 🎯 **Objective**
Simulate isothermal precipitation of **Cementite (Fe₃C)** in:
> **0.8 wt% C steel**

Two scenarios:
1. **300°C for 10 s**
2. **600°C for 10 s**

Outputs for both:
- Average precipitate size vs time
- Nucleation rate vs time
- Number density vs time
- Yield strength trend vs time

---

### ⚙️ **Method Summary**
| Step | Description |
|---|---|
| Package | Demo: Steels and Fe-Alloys |
| Composition | 0.8 wt% C + Fe balance |
| Initial Phase | **BCC_A2#1** |
| Tool | Precipitation Non-Equilibrium Calculator |
| Time | 10 seconds (both cases) |

---

## 🔁 Comparative Results — 300°C vs 600°C

### 📊 **Nucleation Rate**
| Temperature | Nucleation Behavior |
|---|---|
| **300°C** | High → sharp drop after ~10⁻⁵ s |
| **600°C** | Very high → sharp drop after ~10⁻⁷ s |

> Higher T → higher initial nucleation due to increased atomic mobility

---

### 📏 **Average Precipitate Size**
| Temperature | Growth Behavior |
|---|---|
| **300°C** | Slow start → Rapid growth after 10⁻⁴ s |
| **600°C** | Negligible early growth → Rapid growth after 10⁻² s |

Diffusion kinetics accelerated at **600°C**, producing larger precipitates faster.

---

### 🔹 **Number Density of Precipitates**
Both temperatures follow:
> Rapid rise → Peak → Gradual decay

Decay caused by **coarsening** (Ostwald ripening).

---

### 💪 **Yield Strength Trends**
| Temperature | Strengthening Behavior |
|---|---|
| **300°C** | Gradual strengthening due to finer precipitates |
| **600°C** | Faster strengthening, higher final strength |

---

## 🔗 Correlation Summary (Mechanical–Microstructural)

> **Nucleation Rate → Precipitate Density → Size → Strength**

- High nucleation → many small particles
- Growth/coarsening → fewer + larger particles
- Precipitates block dislocation motion → ↑ yield strength

At higher temperatures:
- Faster diffusion → larger cementite → higher strengthening rate

---

## 🌡️ Role of Temperature in Precipitation

Temperature controls:
1. **Diffusion rate**
2. **Nucleation activation energy**
3. **Coarsening kinetics**
4. **Mechanical strengthening timeline**

**300°C**
- Low diffusion
- Fine, dense precipitates
- Gradual, stable strengthening

**600°C**
- High diffusion
- Rapid growth & coarsening
- Higher strengthening within short time

---

## 📌 Final Takeaways

| Aspect | Al₃Sc (Report 1) | Cementite (Report 2) |
|---|---|---|
| Geometry | Spherical | Bulk precipitation |
| Control Mechanism | Diffusion-limited | Nucleation + coarsening |
| Strength Mechanism | Precipitation hardening | Precipitation hardening |
| Temperature Role | Solubility + diffusion | Diffusion + coarsening |
| Key Feature | Interface tracking | Mechanical property link |

---


