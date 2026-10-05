# **Nawaz's D&P Level 1 Report**
---
## **Task 01** - Engineer's Swiss Army Knife (MATLAB Onramp)

### Objective
To learn the basics of MATLAB programming and familiarize with its applications in engineering through the MATLAB Onramp course.  

---

### Tools Used
- MATLAB Online (MathWorks)
- MATLAB Onramp Course

---

### Procedure
1. Created a MathWorks account using institutional email.
2. Accessed MATLAB Onramp via MATLAB Academy.
3. Completed all modules including:
   - Variables and expressions
   - Vectors and matrices
   - Indexing
   - Plotting data
4. Performed hands-on coding exercises in MATLAB Online.
5. Completed the course and obtained certification.

---

### Key Learnings
- Learned MATLAB syntax including variable assignment and vector creation
- Performed element-wise operations using .* and ./
- Used indexing techniques like a(1:3)
- Plotted graphs using plot(x,y)
---

### Applications 
- Signal processing and analysis
- Numerical computations
- Data visualization
- Engineering simulations

---

### Result
Successfully completed the MATLAB Onramp course and obtained the certification.

---

### Certificate Of Completion
![Certificate of completion](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Completion_certificate.png?raw=true)      

---    
### Progress report  
![Progress Report](https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/refs/heads/main/Progress_report.png)  

---  
## **Task 02** - SPICEy Code

### Objective
To understand the fundamentals of SPICE (Simulation Program with Integrated Circuit Emphasis) by writing and simulating SPICE netlists for basic digital logic circuits using MOSFETs.
  
---  
  
### Task
Write basic SPICE code for:
1. MOS Inverter
2. AND Gate
3. OR Gate

Platform Used: LTSpice

---

### Theory
SPICE is a circuit simulation language used to describe electronic circuits through text-based netlists. Components, power supplies, inputs, and simulation commands are defined using SPICE syntax, allowing the circuit behaviour to be analysed before hardware implementation.

A MOS inverter is the most fundamental CMOS logic circuit. It consists of complementary NMOS and PMOS transistors and performs logical inversion of the input signal.

AND and OR gates are basic combinational logic circuits that can be implemented using MOS transistor networks. SPICE coding helps in understanding how digital logic is represented and simulated at the transistor level.

---

### Procedure
1. Studied the basic structure and syntax of SPICE netlists.
2. Implemented a CMOS inverter using NMOS and PMOS transistors.
3. Verified the inverter operation by applying a pulsed input signal.
4. Developed SPICE netlists for AND and OR gates.
5. Simulated each circuit in LTSpice.
6. Observed input-output waveforms and verified the truth table behaviour.

---
  
### Results
- Successfully implemented a CMOS inverter using SPICE code.
- Successfully implemented AND gate functionality using MOSFET-based logic.
- Successfully implemented OR gate functionality using MOSFET-based logic.
- Verified the expected output waveforms through LTSpice simulation.

---

### Learning Outcomes
- Understood the purpose and structure of SPICE netlists.
- Learned how MOSFETs are used to implement digital logic circuits.
- Gained experience in LTSpice simulation and waveform analysis.
- Understood the transistor-level implementation of inverter, AND, and OR gates.

---

### Standard Circuits Schematic 
![standard circuits](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/standard_ckts_detailed.png?raw=true)        

--- 
## **Task 03** - Cut, Pass, Repeat

### Objective
To design and analyze a second-order active Band Pass Filter using an operational amplifier and verify its frequency response through LTSpice simulation.

---

### Tools Used
- LTSpice
- Operational Amplifier (Op-Amp)
- Resistors
- Capacitors

---

### Theory
A Band Pass Filter (BPF) is an electronic circuit that allows signals within a specific frequency range to pass while attenuating frequencies outside that range.

A second-order active band pass filter is formed by cascading:
1. A High Pass Filter (HPF)
2. A Low Pass Filter (LPF)

The lower cut-off frequency is determined by the high-pass section, while the upper cut-off frequency is determined by the low-pass section. The region between these frequencies is known as the pass band.

The operational amplifier provides amplification and isolation between the filter stages, improving overall performance and stability.

---

### Design Specifications
- Lower Cut-off Frequency (fL) = 4 kHz
- Upper Cut-off Frequency (fH) = 16 kHz
- Capacitor Value = 10 nF
- Filter Type = Second Order Active Band Pass Filter

---

### Design Calculations

For the High Pass Filter:

R₁ = 1 / (2πfLC)

R₁ = 1 / (2π × 4000 × 10 × 10⁻⁹)

R₁ ≈ 3.9 kΩ

For the Low Pass Filter:

R₂ = 1 / (2πfHC)

R₂ = 1 / (2π × 16000 × 10 × 10⁻⁹)

R₂ ≈ 1 kΩ

Standard resistor values were selected for practical implementation.

---

### Procedure
1. Calculated resistor values using the cut-off frequency equations.
2. Designed the High Pass Filter section for a cut-off frequency of 4 kHz.
3. Designed the Low Pass Filter section for a cut-off frequency of 16 kHz.
4. Combined both stages using an operational amplifier.
5. Simulated the circuit in LTSpice.
6. Performed AC analysis to obtain the frequency response.
7. Verified the pass band between the lower and upper cut-off frequencies.

---

### Results
- Successfully designed a second-order active Band Pass Filter.
- Obtained the required pass band between 4 kHz and 16 kHz.
- Verified filter operation through LTSpice simulation.
- Observed attenuation of frequencies outside the desired pass band.

---

### Learning Outcomes
- Understood the working principle of High Pass and Low Pass filters.
- Learned how cascading HPF and LPF stages produces a Band Pass Filter.
- Gained experience in active filter design using operational amplifiers.
- Learned to perform AC analysis in LTSpice.
- Understood the significance of cut-off frequencies and pass band characteristics.

---

### Band Pass Filter Circuit
![Band Pass Filter Circuit](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/BPF_CKT.png?raw=true)

---

### Frequency Response
![Frequency Response](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/BandPassGraph.png?raw=true)

---
## **Task 04** - From Low to Woah!

### Objective
To understand the working of voltage multipliers using capacitor charge pumps driven by a 555 Timer IC and generate higher DC voltages from a 9V input supply.

---

### Task
1. Design a voltage multiplier circuit to increase a 9V DC input.
2. Use capacitor charge-pump stages driven by a 555 Timer IC.
3. Observe the voltage multiplication effect through simulation.
4. Verify the output voltages obtained at each stage.

Platform Used: LTSpice

---

### Theory
A voltage multiplier is a circuit that converts a low DC voltage into a higher DC voltage using capacitors and diodes. Instead of using a transformer, the circuit stores and transfers charge between capacitors during each switching cycle.

The 555 Timer IC is configured in astable mode to generate a continuous square-wave signal. This signal repeatedly charges and discharges the capacitors through the diode network.

As the capacitors charge, their voltages add together, resulting in a higher output voltage. By cascading multiple charge-pump stages, the output voltage can be increased further.

---

### Components Used
- NE555 Timer IC
- Diodes
- Capacitors
- Resistors
- 9V DC Supply

---

### Procedure
1. Configured the 555 Timer IC in astable mode to generate a square-wave signal.
2. Connected a capacitor-diode network to form the first voltage multiplier stage.
3. Simulated the circuit and observed the voltage increase at the intermediate node.
4. Added another multiplier stage by cascading additional capacitors and diodes.
5. Simulated the complete circuit in LTSpice.
6. Measured the voltages at different stages and analysed the output waveform.

---

### Observations
- The first voltage multiplier stage increased the input voltage from 9V to approximately 16.6V.
- The second multiplier stage further increased the voltage to approximately 24.4V.
- The output voltage gradually increased as the capacitors charged.
- Small ripple voltages were observed due to the charging and discharging cycles of the capacitors.

---

### Results
- Successfully implemented a voltage multiplier circuit using a 555 Timer IC.
- Obtained approximately 16.6V at the first multiplier stage from a 9V input supply.
- Obtained approximately 24.4V at the final multiplier stage by cascading charge-pump stages.
- Verified the voltage multiplication effect through LTSpice simulation.

---

### Learning Outcomes
- Understood the working principle of capacitor charge pumps.
- Learned how diodes control the direction of current flow during charging cycles.
- Understood how cascading stages increases the output voltage.
- Gained experience in simulating voltage multiplier circuits using LTSpice.
- Learned the practical effects of diode voltage drops and output ripple.

---

### 555 Timer Voltage Multiplier Circuit

![555 Timer Voltage Multiplier](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Voltage_Multiplier.png?raw=true)

---

### Simulation Results

![Voltage Multiplier Waveforms](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/VTG_MUL_GRAPH.png?raw=true)

---