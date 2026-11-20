# Semiconductor Devices and Circuits (SDC) — Complete Course Study Guide

> **Bharati Vidyapeeth (Deemed to be University) College of Engineering, Pune**  
> **Department of Electronics and Telecommunication Engineering**  
> **Course:** Semiconductor Devices & Circuits (SDC) · B.Tech Semester III (NEP 2020)  
> **Faculty Alignment:** Dr. R. B. Ghongade Lecture Notes & Examination Solutions

---

## 🌐 Live GitHub Pages Link

The entire 6-unit master compilation is hosted live via GitHub Pages at:
👉 **[https://n2v5y7t.github.io/SDC/](https://n2v5y7t.github.io/SDC/)**

*(Opening this link renders the entire complete master study guide directly in your browser with zero downloads, dark/light theme switching, interactive SVG circuits, and calculators.)*

---

## 📖 Overview

This repository contains the complete, self-contained, interactive digital study guide covering **all 6 units** of the Semiconductor Devices & Circuits (SDC) syllabus.

Every unit follows an intuitive 5-pillar pedagogical architecture:
1. **Physical Intuition:** Intuitive analogies, mental pictures, and device physics.
2. **Circuit Schematic:** Self-contained inline vector SVG circuits with interactive parameter nodes.
3. **Mathematical Derivations:** Step-by-step rigorous analytical proofs with formatted fractions, square roots ($\sqrt{X}$), sub/superscripts, and Greek symbols.
4. **Solved Numerical Design Walkthroughs:** Exact calculations based on Dr. R. B. Ghongade's lecture problems, standard E12 resistor/capacitor value selections, and safety margins.
5. **Previous Year Exam Paper (PYQ) Maps:** Complete solution blueprints and marking rubrics for Summer 2026, Winter 2025, and SDC-I/II semester exams.

---

## 🚀 Repository Structure & Files

| File | Description | Size |
| :--- | :--- | :--- |
| **[`index.html`](./index.html)** | **Root Entry Point for GitHub Pages:** Full 6-unit compilation with multi-unit navigation | ~727 KB |
| **[`SDC_Complete_Study_Guide.html`](./SDC_Complete_Study_Guide.html)** | Master compiled single file (identical to `index.html`) | ~727 KB |
| **[`SDC Unit1.html`](./SDC%20Unit1.html)** | **Unit 1:** BJT Amplifiers (AC Load Line, $h$-parameters, CE/CC/CB Analysis & Design) | ~149 KB |
| **[`SDC Unit2.html`](./SDC%20Unit2.html)** | **Unit 2:** JFET & MOSFET Amplifiers (Depletion/Enhancement, CS/CD/CG, CMOS Inverter) | ~153 KB |
| **[`SDC Unit3.html`](./SDC%20Unit3.html)** | **Unit 3:** Multistage BJT Amplifiers (Miller Effect, RC/Direct/Transformer Coupling, Cascode & Darlington) | ~118 KB |
| **[`SDC Unit4.html`](./SDC%20Unit4.html)** | **Unit 4:** Feedback Amplifiers (4 Topologies, Desensitivity, Bandwidth Extension, BJT Derivations) | ~80 KB |
| **[`SDC Unit5.html`](./SDC%20Unit5.html)** | **Unit 5:** Power Amplifiers (Class A/B/AB/C/D, 78.5% Push-Pull, Complementary-Symmetry, Heat Sinks) | ~146 KB |
| **[`SDC Unit6.html`](./SDC%20Unit6.html)** | **Unit 6:** BJT Current Mirrors & Differential Amplifiers (Widlar/Wilson, Split-Supply, CMRR, $\tanh$ Transfer) | ~131 KB |

---

## ⚙️ How GitHub Pages is Configured

To ensure GitHub Pages displays **only the master whole compilation**:
1. `index.html` is located directly at the repository root and contains the full combined guide across all 6 units.
2. A `.nojekyll` file is placed in the root to bypass Jekyll processing, preventing template or math syntax parsing conflicts.
3. An automated GitHub Actions workflow (`.github/workflows/pages.yml`) is included to deploy the site to GitHub Pages on every push.

### Enabling GitHub Pages in Repository Settings:
If GitHub Pages is not yet enabled on your repository:
1. Go to **Settings** on `https://github.com/N2V5Y7T/SDC`.
2. On the left sidebar, click **Pages** (under the "Code and automation" section).
3. Under **Build and deployment**:
   - **Option A (GitHub Actions - Recommended):** Set **Source** to **GitHub Actions**. The automated workflow will deploy it immediately.
   - **Option B (Deploy from branch):** Set **Source** to **Deploy from a branch**, select branch **`main`**, and folder **`/ (root)`**, then click **Save**.
4. Your site will be live at: **`https://n2v5y7t.github.io/SDC/`**

---

## 📚 Unit Breakdown & Syllabus Coverage

### Unit 1: BJT Amplifiers
- Physical transistor mechanisms, amplification conditions, and DC/AC load line derivation
- Two-port network conventions, $h$-parameter linear model and conversion formulas
- Complete small-signal analysis of CE, CC (emitter follower), and CB configurations ($A_v, A_i, R_i, R_o$)
- Single-stage RC-coupled CE amplifier practical design procedure with bypass and coupling capacitor design
- Large-signal considerations, transistor as a saturated switch, thermal physics, and heat sink derating

### Unit 2: JFET and MOSFET Amplifiers
- JFET construction, pinch-off mechanism, Shockley transfer equation, and dynamic parameters ($g_m, r_d, \mu$)
- JFET small-signal equivalent circuit and Common Source (CS), Common Drain (CD), Common Gate (CG) analysis
- Enhancement and Depletion MOSFET physics, inversion layer formation, and square-law characteristics
- MOSFET amplifiers (CS with bypass, unbypassed, CD source follower), resistive-load inverter, and CMOS inverter
- Power MOSFETs (VMOS, DMOS), parasitic capacitances ($C_{gs}, C_{gd}$), and high-frequency roll-off

### Unit 3: Multistage BJT Amplifiers
- Low-, mid-, and high-frequency response regions and logarithmic decibel scale
- High-frequency hybrid-$\pi$ ($\text{Giacoletto}$) model and parameter definitions ($r_{b'e}, r_{bb'}, g_m, C_e, C_c$)
- Miller's Theorem: input capacitance multiplication ($C_M = C_f(1 - A_v)$) and output admittance formulation
- Gain-bandwidth trade-off in cascade amplifiers ($BW_n = BW_1 \sqrt{2^{1/n} - 1}$)
- Coupling techniques: RC-coupled, Direct-coupled, Transformer-coupled, Darlington pair ($\beta^2$), and Cascode (CE-CB)

### Unit 4: Feedback Amplifiers
- Fundamental feedback concept: open-loop $A$, feedback factor $\beta$, closed-loop gain $A_f = \frac{A}{1 + A\beta}$
- The 4 feedback topologies: Voltage-Series, Current-Series, Current-Shunt, and Voltage-Shunt
- 3-step practical topology identification rule (output sampling type & input mixing node)
- Benefits of negative feedback: gain desensitization, bandwidth extension ($f_{H(f)} = f_H(1+A\beta)$), distortion and noise reduction
- Exhaustive small-signal analysis and worked BJT design problems for all 4 topologies

### Unit 5: Power Amplifiers & Large-Signal Analysis
- Power amplifier need, classification by conduction angle: Class A ($360^\circ$), Class B ($180^\circ$), Class AB, Class C ($<180^\circ$), Class D (switching/PWM)
- Series-Fed Class A: maximum theoretical efficiency $\eta_{max} = 25\%$, Figure of Merit $FM = 2$
- Transformer-Coupled Class A: inductive kick swinging $V_{CE}$ to $2V_{CC}$, impedance matching, $\eta_{max} = 50\%$
- Class B Push-Pull: anti-phase drive, even-harmonic cancellation, maximum efficiency $\eta_{max} = \frac{\pi}{4} = 78.54\%$
- Transistor dissipation peak at $V_p = \frac{2}{\pi} V_{CC} \approx 0.636 V_{CC}$ with $P_{D(max)} = \frac{2V_{CC}^2}{\pi^2 R_L'}$
- Crossover distortion at $0.7\text{ V}$ $V_{BE}$ cut-in threshold and Class AB diode biasing elimination
- Transformerless output (OTL): Complementary-Symmetry Class AB and Quasi-Complementary (Lin) topology
- Harmonic distortion: 3-point and 5-point analysis, Total Harmonic Distortion ($THD$), and thermal heatsink physics ($\theta_{JA}$)

### Unit 6: BJT Current Mirrors and Differential Amplifiers
- Need for IC constant-current biasing; basic two-transistor current mirror and finite $\beta$ error ($I_O = \frac{I_{ref}}{1 + 2/\beta}$)
- Widlar current source for low micro-ampere biasing ($I_O R_E = V_T \ln(I_{ref}/I_O)$)
- Wilson current mirror: triple-transistor feedback canceling base currents ($2/\beta^2$ error) and high $R_o \approx \beta r_o / 2$
- Shortcomings of standard CE amplifiers for DC/low-frequency amplification (drift, $V_{BE}$ thermal shifts, capacitor sizes)
- Differential amplifier physics: emitter-coupled pair with split dual power supply ($\pm V_{EE}, V_{CC}$)
- Differential mode (anti-phase) vs Common mode (in-phase) operation and rejection
- The 4 diff amp configurations: Dual-Input Balanced-Output (DIBO), Dual-Input Unbalanced-Output (DIUO), Single-Input Balanced-Output (SIBO), Single-Input Unbalanced-Output (SIUO)
- Differential voltage gain $A_d = \frac{h_{fe} R_C}{2 h_{ie}}$, common-mode gain $A_c = \frac{-h_{fe} R_C}{h_{ie} + 2(1+h_{fe})R_E}$
- Common Mode Rejection Ratio (CMRR) and tail improvement using constant-current sources
- Large-signal nonlinear transfer dynamics: differential pair hyperbolic tangent transfer characteristics ($\tanh(v_{id}/2V_T)$)

---

## 🛠️ Technical Features
- **Zero External Dependencies:** Built with pure vanilla HTML, modern CSS flex/grid, and JavaScript. Renders 100% offline.
- **Buttery-Smooth Navigation:** Uses native container scroll positioning without browser-kinetic-cancellation bugs.
- **Mathematical Typography:** Renders square roots ($\sqrt{X}$ with full vinculum), fraction bars, and mathematical subscripts natively.
- **Dark/Light Theme:** Integrated toggle with automatic system preference detection.
- **Progress Tracking:** Interactive completion checkboxes with persistent `localStorage` progress memory.

---

*Prepared for B.Tech E&TC Semester III Students · Bharati Vidyapeeth (DU) COE, Pune*
