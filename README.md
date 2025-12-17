# Elector's-Tiny-Solar-Power-Supply-PCB
# Elektor’s Solar Power Supply – Learning-Oriented Redesign

## 1. Project Overview
This project is a learning-focused redesign of **Elektor’s Tiny Solar Power Supply**. The aim is to understand the fundamentals of solar energy harvesting and low-power power supply design through hands-on schematic capture and PCB layout.

The entire circuit and PCB were redesigned from scratch using **KiCad EDA**, while referring to the original Elektor concept **strictly for educational and learning purposes**. This project emphasizes clarity, simplicity, and real-world design thinking rather than product optimization.

---

## 2. Key Learning Objectives
- Understanding **solar input conditioning** and handling variable input sources  
- Learning **power regulation basics** for low-power applications  
- Developing **component selection reasoning** based on electrical and practical constraints  
- Applying **practical PCB layout considerations** such as trace routing, grounding, and component placement  

---

## 3. Tools & Software Used
- **KiCad EDA**
  - Schematic Editor  
  - PCB Layout Editor  
  - 3D Viewer  

---

## 4. Project Files
- Schematic design files (`.kicad_sch`)  
- PCB layout files (`.kicad_pcb`)  
- 3D render images  
- Manufacturing-ready Gerber files  

---

## 5. Block-Level Working Explanation
The system starts with a **solar panel** as the primary energy source. Since solar output varies with light conditions, the input stage conditions and stabilizes this energy before it is used further.

The conditioned solar input is then passed to a **DC-DC regulation stage**, which converts the variable input voltage into a usable and stable output suitable for low-power electronic circuits. Passive components around the regulator help improve stability and efficiency.

Finally, the regulated output is made available through the output terminals, allowing it to power small loads or act as a learning reference for energy-harvesting power supplies.

This block-level flow helps beginners understand how energy moves through the system without diving into complex mathematical analysis.

---

## 6. Bill of Materials (BOM)

| S.No | Reference | Component Type        | Value / Part Number        | Footprint     | Quantity | Description |
|------|-----------|----------------------|----------------------------|---------------|----------|-------------|
| 1    | U1        | DC-DC Boost Converter| AP3015AKTR-G1               | SOT-23-5     | 1        | Step-up DC-DC converter |
| 2    | L1        | Inductor             | 10µH (LQM15AN103B0D)        | 0603         | 1        | Energy storage inductor |
| 3    | D1        | Schottky Diode       | SS14                       | SMA           | 1        | Output rectifier |
| 4    | D2        | Schottky Diode       | SS14                       | SMA           | 1        | Input protection |
| 5    | Q1        | N-Channel MOSFET     | 2N7002                     | SOT-23        | 1        | Load / power control |
| 6    | R1        | Resistor             | 1MΩ                        | 0603          | 1        | Feedback resistor |
| 7    | R2        | Resistor             | 604kΩ                      | 0603          | 1        | Feedback resistor |
| 8    | R3        | Resistor             | 100kΩ                      | 0603          | 1        | Gate pull-up |
| 9    | R4        | Resistor             | 10Ω                        | 0603          | 1        | Current limiting |
| 10   | C1        | Ceramic Capacitor    | 4.7µF, 50V, X7R            | 0805          | 1        | Input bypass capacitor |
| 11   | C2        | Ceramic Capacitor    | 22µF, 10V, X7R             | 1206          | 1        | Output bulk capacitor |
| 12   | C3        | Ceramic Capacitor    | 10µF, 50V, X7R             | 0805          | 1        | Output filtering |
| 13   | J1        | Connector            | Conn_01x02_Pin             | Through-hole  | 1        | Output connector |
| 14   | J2        | Connector            | Conn_01x02_Pin             | Through-hole  | 1        | Battery connector |
| 15   | J4        | Connector            | Conn_01x02_Pin             | Through-hole  | 1        | Solar panel input |
| 16   | SW1       | Switch               | ON/OFF (Conn_01x02_Pin)    | Through-hole  | 1        | Power enable switch |


---

## 7. Images & Renders

- **Schematic**  
 <img width="1082" height="746" alt="Screenshot 2025-12-06 165636" src="https://github.com/user-attachments/assets/7100dff9-c44d-4768-9d88-297e87470370" />


- **PCB Layout**  
 <img width="1542" height="806" alt="Screenshot 2025-12-06 165503" src="https://github.com/user-attachments/assets/ee0b36e1-6739-44f1-a46b-cc0b1ca534c3" />


- **3D View**  
  <img width="1723" height="892" alt="Screenshot 2025-12-07 211327" src="https://github.com/user-attachments/assets/35b297e6-8175-4dc4-a803-1cc63b77438f" />
  <img width="1723" height="938" alt="Screenshot 2025-12-07 211958" src="https://github.com/user-attachments/assets/649a3b8d-ca07-40b3-9f39-9781ce2530e9" />



---

## 8. Disclaimer
This project is intended **solely for learning and educational purposes**. It is not designed or validated for commercial or critical applications.

The original concept is **inspired by Elektor**, and all redesign work presented here is independently implemented to improve understanding of solar-powered circuit design and PCB development.

---

## 9. Author
- **Name:** Yukesh S  
- **Toolchain:** KiCad EDA  

