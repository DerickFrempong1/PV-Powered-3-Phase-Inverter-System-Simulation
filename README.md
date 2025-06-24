## 🔋 PV-Powered 3-Phase Inverter System Simulation (MATLAB/Simulink)

This project presents a MATLAB/Simulink model of a **PV-powered smart microgrid system** consisting of a **Boost Converter**, a custom-built **3-Phase Inverter**, and a **Load and Filter Section**. It is designed to demonstrate DC-AC conversion using pulse-width modulation (PWM) for renewable energy applications.



### ⚙️ System Components

#### ✅ 1. PV Array

* Acts as the primary DC source.
* Configured with variable irradiance (1500 W/m²) and temperature (25°C).

#### ✅ 2. Boost Converter

* Increases the DC voltage from the PV array to a suitable level for inversion.
* Comprises:

  * Series RLC Branch (Inductor)
  * IGBT switch (controlled via Pulse Generator)
  * Diode and Output Capacitor

#### ✅ 3. Gate Control Logic

* Generates PWM signals for six IGBT switches.
* Uses reference sine waves and a carrier triangle waveform.
* Includes relational operators and NOT gates for complementary switching.

#### ✅ 4. 3-Phase Inverter

* Custom-built using discrete IGBT/Diode blocks (replacing the Universal Bridge).
* Converts boosted DC into 3-phase AC.

#### ✅ 5. Load and Filter Section

* RLC filters smooth the inverter output.
* Connected to a balanced 3-phase resistive-inductive load.

#### ✅ 6. Measurement and Scopes

* Voltage probes are placed across PV output, DC link, and AC output.
* Scopes (`Scope1`, `Scope2`, `Scope3`) visualize system performance.



### 🔍 Simulation Configuration

* **Solver:** Continuous
* **Control Mode:** Open-loop PWM
* **Software:** MATLAB/Simulink (tested on R2024b or later)



### 📁 File Contents

| File                     | Description                        |
| ------------------------ | ---------------------------------- |
| `FINAL INVERTER.png`     | Full schematic screenshot          |
| `PV_3Phase_Inverter.slx` | Simulink model (not included here) |
| `README.md`              | Project documentation (this file)  |


### 📌 Applications

* Renewable energy integration
* Microgrid control systems
* Power electronics teaching/demonstration
* Graduate school project portfolio


### ✍️ Author

**Derick Ameyaw Frempong**
Power Systems Enthusiast | Electrical/Electronic Engineer
[Ghana Ports and Harbours Authority]

