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

## **Task 05** - The Power Shuffle: Buck-Boost Edition

### Objective
To understand the working of DC-DC converters and design Buck and Boost converters using LTSpice.

---

### Task
1. Design a Boost Converter to step up 1.5V DC to 5V DC.
2. Design a Buck Converter to step down 12V DC to 5V DC.
3. Simulate both circuits in LTSpice and observe the output voltage.

Platform Used: LTSpice

---

### Theory
DC-DC converters are switching circuits used to convert one DC voltage level into another.

A Boost Converter increases the input voltage to a higher output voltage. It mainly consists of an inductor, switch, diode, and capacitor. When the switch is ON, energy is stored in the inductor. When the switch turns OFF, the inductor releases its stored energy through the diode to the capacitor and load, increasing the output voltage.

A Buck Converter works in the opposite way and reduces a higher DC input voltage to a lower DC output voltage. The switch continuously turns ON and OFF, and the average output voltage depends mainly on the duty cycle of the switching waveform.

---

### Boost Converter

The Boost Converter was designed to increase the input voltage from 1.5V to approximately 5V.

For an ideal Boost Converter,

Vout = Vin / (1 - D)

where,

D = Duty Cycle

Rearranging,

D = 1 - (Vin / Vout)

For Vin = 1.5V and Vout = 5V,

D = 1 - (1.5 / 5)

D = 0.7

Therefore, the required duty cycle is approximately 70%.

---

### Buck Converter

The Buck Converter was designed to decrease the input voltage from 12V to approximately 5V.

For an ideal Buck Converter,

Vout = D × Vin

Therefore,

D = Vout / Vin

For Vin = 12V and Vout = 5V,

D = 5 / 12

D ≈ 0.417

Therefore, the required duty cycle is approximately 41.7%.

---

### Components Used
- MOSFET as switching device
- Inductor
- Diode
- Capacitor
- Resistors
- DC Voltage Source
- Pulse Source / 555 Timer switching source

---

### Procedure
1. Calculated the required duty cycle for both the Buck and Boost converters.
2. Designed the Boost Converter using an inductor, MOSFET, diode, and capacitor.
3. Applied a 1.5V DC input and adjusted the switching waveform to obtain approximately 5V at the output.
4. Designed the Buck Converter using the same basic switching components.
5. Applied a 12V DC input and adjusted the duty cycle to obtain approximately 5V at the output.
6. Performed transient analysis in LTSpice.
7. Observed the switching waveform and output voltage for both converters.
8. Tested the switching circuit using both a PULSE source and a 555 Timer based signal.

---

### Observation With 555 Timer
While testing the switching source, I noticed a difference between the LTSpice PULSE source and the 555 Timer output.

The PULSE source was configured to start from LOW and then switch to HIGH.

However, the 555 Timer output started from HIGH when the simulation began.

This happens because at power-on the timing capacitor of the 555 Timer is initially discharged. Its voltage is below 1/3 of Vcc, which sets the internal latch and makes the output HIGH.

Because of this, the switching waveform generated using the 555 Timer started in the HIGH state, whereas the PULSE source started from the LOW state.

If a LOW output is required at the beginning of the simulation, the RESET pin can be kept LOW briefly during startup or the timing capacitor can be given an initial voltage using the `.ic` directive in LTSpice.

---

### Results
- Successfully simulated a Boost Converter with an input of 1.5V and an output close to 5V.
- Successfully simulated a Buck Converter with an input of 12V and an output close to 5V.
- Observed the effect of duty cycle on the output voltage.
- Compared the switching behaviour of a PULSE source and a 555 Timer based clock source.
- Observed that the 555 Timer naturally starts with its output HIGH during power-on.

---

### Learning Outcomes
- Understood the working principle of Buck and Boost converters.
- Learned how energy is stored and released by an inductor in switching converters.
- Understood the relationship between duty cycle and output voltage.
- Learned how MOSFETs are used as high-speed switches in DC-DC converters.
- Gained experience in transient analysis using LTSpice.
- Understood the difference between an ideal PULSE source and the startup behaviour of a practical 555 Timer circuit.

---

### Boost Converter Circuit

![Boost Converter Circuit](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Boost_converter.png?raw=true)

---

### Boost Converter Output

![Boost Converter Output](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Boost_WF.png?raw=true)

---

### Buck Converter Circuit

![Buck Converter Circuit](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Buck_NMOS.png?raw=true)

---

### Buck Converter Output

![Buck Converter Output](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Buck_WF.png?raw=true)

---

### Buck Converter Circuit (555 Timer Based Switching Source)

![Buck Converter Circuit](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Buck_555.png?raw=true)

---

### Buck Converter Output Waveform

![Buck Converter Output](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/Buck_555_WF.png?raw=true)

---

### Conclusion
The Buck and Boost converters were successfully designed and simulated in LTSpice. The Boost Converter increased the 1.5V input to approximately 5V, while the Buck Converter reduced the 12V input to approximately 5V. The simulations also helped in understanding the importance of duty cycle and the switching behaviour of the circuit. While testing the switching sources, a difference in startup behaviour was observed between the LTSpice PULSE source and the 555 Timer, with the 555 Timer starting in the HIGH state due to the initially discharged timing capacitor.

---  

## **Task 06** - 4 Bits to Rule Them All

### Objective
To design and implement a 4-bit Arithmetic Logic Unit (ALU) capable of performing arithmetic and logical operations using basic digital logic components in CircuitVerse.

---

### Tools Used
- CircuitVerse
- Digital Logic Design Concepts

---

### Task
Design and implement a 4-bit ALU capable of performing:

1. 4-bit Addition
2. 4-bit Subtraction using 2's Complement
3. 4-bit AND Operation
4. 4-bit OR Operation
5. 4-bit XOR Operation
6. 4-bit NOT Operation (Bonus)

The ALU should use control signals to select the required operation and display the corresponding output.

---

### Theory

An Arithmetic Logic Unit (ALU) is the computational core of a digital system. It performs arithmetic and logical operations on binary data.

A 4-bit ALU accepts two 4-bit inputs and processes them based on control signals. Arithmetic operations such as addition and subtraction are performed using adder circuits, while logical operations are implemented using logic gates.

Subtraction is achieved using the 2's complement method, where the second operand is inverted and a carry of 1 is added. This allows subtraction to be performed using the same adder hardware used for addition.

Control lines are used to select the desired operation, making the ALU a programmable combinational circuit.

---

### Procedure

1. Designed a 4-bit ripple carry adder using Full Adders.
2. Verified correct carry propagation and arithmetic addition.
3. Modified the adder circuit to perform subtraction using the 2's complement technique.
4. Implemented 4-bit AND, OR, XOR and NOT circuits using logic gates.
5. Designed multiplexing logic to select the required operation based on control signals.
6. Combined all arithmetic and logical blocks into a single ALU architecture.
7. Tested all possible operations with different input combinations.
8. Verified outputs for correctness.

---

### Individual Functional Blocks

<table>
<tr>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_ADD.png" width="300"></td>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_ADD_SUB.png" width="300"></td>
</tr>

<tr>
<td align="center">4-Bit Adder</td>
<td align="center">4-Bit Adder/Subtractor</td>
</tr>

<tr>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_AND.png" width="300"></td>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_OR.png" width="300"></td>
</tr>

<tr>
<td align="center">4-Bit AND</td>
<td align="center">4-Bit OR</td>
</tr>

<tr>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_XOR.png" width="300"></td>
<td><img src="https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/4_BIT_NOT.png" width="300"></td>
</tr>

<tr>
<td align="center">4-Bit XOR</td>
<td align="center">4-Bit NOT</td>
</tr>
</table>

---

### ALU Design (Using 2 Select Lines)

![ALU Stage 2](https://raw.githubusercontent.com/nawazhussainhs/Marvel_Level_1_Images/main/ALU_2_SL.png)

---

### Final 4-Bit ALU

![Final ALU](https://github.com/nawazhussainhs/Marvel_Level_1_Images/blob/main/ALU_3SL&FLAG.png?raw=true)

---
  
### Sample Verification Table

For testing the ALU, the following inputs were used:

| Input A | Input B |
|----------|----------|
| 1011 | 0110 |

| Select Lines | Operation | Output |
|-------------|-----------|---------|
| 000 | Addition (A + B) | 0001 (Carry = 1) |
| 001 | Subtraction (A - B) | 0101 |
| 010 | AND | 0010 |
| 011 | OR | 1111 |
| 100 | XOR | 1101 |
| 101 | NOT A | 0100 |

The obtained outputs matched the expected results for all tested operations.  
  
---  

### Working

- The 4-bit adder performs binary addition of two 4-bit inputs.
- The subtractor uses XOR gates and a carry-in of 1 to generate the 2's complement of the second operand.
- AND, OR and XOR blocks perform bitwise logical operations.
- The NOT block inverts each bit of the selected input.
- Control lines determine which operation output is routed to the final ALU output.
- The ALU produces the required result while also handling carry generation during arithmetic operations.

---

### Results

- Successfully designed a 4-bit Adder.
- Successfully implemented a 4-bit Adder/Subtractor using 2's complement.
- Successfully implemented 4-bit AND, OR and XOR logic operations.
- Successfully implemented 4-bit NOT operation.
- Successfully integrated all functional blocks into a single ALU architecture.
- Verified correct operation through simulation and testing in CircuitVerse.
- Verified ALU functionality using test inputs A = 1011 and B = 0110 for all supported operations.

---

### Learning Outcomes

- Understood the architecture of an ALU.
- Learned how arithmetic operations are implemented using Full Adders.
- Understood subtraction using the 2's complement method.
- Learned implementation of bitwise logical operations.
- Gained experience in hierarchical digital circuit design.
- Learned how control signals are used to select ALU operations.
- Improved understanding of combinational logic system design.

---
  
### CircuitVerse Project

CircuitVerse Project Link:

[View 4-Bit ALU Project](https://circuitverse.org/users/468542/projects/arithmetic-logic-unit-68bc0793-3dd8-4d7c-bd84-a7188b9f7a7c)  
  
---
  

### Conclusion

A fully functional 4-bit ALU was successfully designed and implemented in CircuitVerse. The ALU performs arithmetic operations such as addition and subtraction along with logical operations including AND, OR, XOR and NOT. The project provided practical exposure to digital circuit design, control logic implementation and modular system integration.