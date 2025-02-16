# Design of Two Stages Operational Amplifier

## Project Overview:
This project involves the design and simulation of a two-stage operational amplifier (OpAmp) based on specific electrical and performance specifications. The primary goal is to meet the required specifications such as DC gain, GBW, phase margin, and output swing. The design is based on hand calculations, MATLAB simulations, and LTspice simulations.

## Key Specifications:
- **DC Gain**: 48dB
- **Gain Bandwidth (GBW)**: 50 MHz
- **Phase Margin (PM)**: > 70°
- **Output Swing**: > 0.7V
- **Load Capacitance (CL)**: 3pF
- **Compensation Capacitor (CM)**: 0.75pF

## Design Approach:
The OpAmp was designed in MATLAB and LTspice, utilizing hand calculations for transistor sizing and biasing. Various parameters such as the gate-source voltage (Vgs), drain-source voltage (Vds), and current (Ids) were determined based on the provided specifications.

### Key Steps:
1. **Transistor Sizing**: The transistor dimensions (W and L) were selected to meet the desired operating points.
2. **Biasing**: The current for the biasing transistors was calculated, and the corresponding gate-source voltages were determined.
3. **Stability and Frequency Compensation**: The design uses a compensation capacitor (CM) to ensure stability and meet the required phase margin.
4. **Simulation**: The design was simulated in MATLAB for frequency response, noise contribution, and linearity analysis. LTspice was used for simulating the full circuit and generating detailed noise measurements and gain responses.

## Features:
- **Simulation & Design**: The OpAmp design was simulated using MATLAB and LTspice for various metrics such as frequency response, noise, and gain.
- **Design Calculations**: Hand calculations were used for sizing transistors and determining the stability criteria.
- **Compensation Network**: A compensation network was implemented to improve the phase margin and ensure the desired performance.

## Installation:
To replicate this project, you need:

1. **MATLAB**: To run the simulation scripts.
2. **LTspice**: For detailed circuit simulations.
3. **UMC65 Process Models**: For transistor models and simulation setup.

### MATLAB Installation:
1. Install MATLAB on your machine.
2. Download the `UMC65_RVT.mat` file and add it to the project directory.
3. Run the `OpAmp_design.m` script to simulate and analyze the OpAmp.

### LTspice Installation:
1. Download and install LTspice from Linear Technology.
2. Import the provided LTspice netlist to simulate the OpAmp circuit.

## Results:
The project successfully meets the specifications in both the hand calculations and simulations.
- **DC Gain**: 48dB
- **Phase Margin**: 90.15°
- **Gain-Bandwidth**: 51 MHz
- **Output Swing**: > 0.7V
- **Total Noise**: 0.000457165 Vrms

## Conclusion:
The two-stage operational amplifier design achieved the required specifications and passed all tests performed using MATLAB and LTspice simulations. The compensation network improved the phase margin, and the noise analysis showed optimal performance.
