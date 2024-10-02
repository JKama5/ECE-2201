# ECE-2201
Microelectronics

# Cheat Sheet:

## Chapter 3: Semiconductors
### Key Concepts
- **Intrinsic Semiconductor**: Pure, \( n = p = n_i \).
- **Doped Semiconductor**:
  - **n-type**: Donor atoms increase electron concentration.
  - **p-type**: Acceptor atoms increase hole concentration.

- **Current Mechanisms**:
  - **Drift Current**: \( J_{\text{drift}} = q n \mu_n E \)
  - **Diffusion Current**: \( J_{\text{diff}} = q D_n \frac{d n}{d x} \)

- **pn Junction**:
  - **Forward Bias**: Decreases depletion region, allows current.
  - **Reverse Bias**: Increases depletion region, little current flows.
  - **Diode Current**: \( I = I_s \left( e^{\frac{V}{nV_T}} - 1 \right) \)

- **Thermal Voltage**: \( V_T = \frac{kT}{q} \approx 26 \text{ mV at room temperature} \)

---

## Chapter 4: Diodes
### Key Concepts
- **Ideal Diode Model**:
  - **Forward Bias**: \( V_D > 0 \), conducts.
  - **Reverse Bias**: \( V_D < 0 \), blocks.

- **Real Diode Models**:
  - **Constant Voltage Drop Model**: \( V_D \approx 0.7 \text{ V (Silicon)} \)
  - **Small-Signal Resistance**: \( r_d = \frac{V_T}{I_D} \)

- **Zener Diodes**:
  - **Operation in Reverse Breakdown**: \( V_Z \approx V_{breakdown} \)
  - **Voltage Regulation**: Maintains \( V_Z \) under varying load.

- **Key Applications**:
  - **Rectifier Circuits**:
    - **Half-Wave**: Uses single diode.
    - **Full-Wave**: Uses multiple diodes or bridge configuration.

---

## Chapter 5: MOSFETs
### Key Concepts
- **MOSFET Regions of Operation**:
  - **Cutoff**: \( V_{GS} < V_T \) (No current).
  - **Triode**: \( V_{GS} > V_T \), \( V_{DS} < V_{GS} - V_T \).
  - **Saturation**: \( V_{GS} > V_T \), \( V_{DS} \geq V_{GS} - V_T \).

- **Drain Current Equations**:
  - **Triode Region**: \( I_D = k' \left( \frac{W}{L} \right) \left[ (V_{GS} - V_T)V_{DS} - \frac{V_{DS}^2}{2} \right] \)
  - **Saturation Region**: \( I_D = \frac{k'}{2} \left( \frac{W}{L} \right) (V_{GS} - V_T)^2 \)

- **Transconductance**: 
  - \( g_m = \frac{2 I_D}{V_{GS} - V_T} = \frac{2 I_D}{V_{OV}} \)

- **MOSFET Parameters**:
  - \( V_{OV} = V_{GS} - V_T \): Overdrive voltage.

- **Small-Signal Model**:
  - **Voltage Gain**: \( A_v = -g_m R_D \)
  - **Input Resistance**: High, typically \( R_{in} \approx \infty \)

---

## Chapter 7: Transistor Amplifiers
### Key Concepts
- **Common Amplifier Configurations**:
  - **Common-Source (CS)**: High gain, moderate input impedance.
    - **Voltage Gain**: \( A_v = -g_m R_D \)
  - **Common-Gate (CG)**: Low input impedance, good for wide bandwidth.
  - **Source Follower (Common-Drain)**: Buffer, high input and low output impedance.
    - **Voltage Gain**: \( A_v \approx 1 \)

- **Biasing Techniques**:
  - **Voltage Divider Bias**: Common for ensuring a stable \( V_{GS} \) value.
  - **Source Degeneration**: Adds resistance in source leg to stabilize gain.

- **Small-Signal Models**:
  - MOSFETs and BJTs can be approximated by:
    - **\( g_m \)**: Transconductance, governs the current control.
    - **\( r_o \)**: Output resistance, typically \( r_o \approx \infty \) for ideal.

- **Important Small-Signal Parameters**:
  - **Input Resistance (\( R_{in} \))**: For CS amplifier, \( R_{in} \approx \infty \)
  - **Output Resistance (\( R_{out} \))**: \( R_{out} = R_D \parallel r_o \)

- **Frequency Response**:
  - **Bandwidth** and **Gain-Bandwidth Product**: Important in amplifier performance.

---

### Quick References:
- **Thermal Voltage**: \( V_T = 26 \text{ mV at room temperature} \)
- **Diode Equation**: \( I = I_s \left( e^{\frac{V}{nV_T}} - 1 \right) \)
- **MOSFET Saturation Current**: \( I_D = \frac{k'}{2} \left( \frac{W}{L} \right) (V_{GS} - V_T)^2 \)
- **Common-Source Gain**: \( A_v = -g_m R_D \)
