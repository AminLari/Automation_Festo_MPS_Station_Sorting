# Festo MPS Sorting Station Automation

## Overview
Automation of the **Festo MPS Sorting Station** using **Siemens TIA Portal** and **S7-1200 PLC**.  
The system classifies workpieces by **material** and **color**, using a sequence of sensor readings and actuator controls coordinated through a modular PLC program.

<p> 
  <img src="https://github.com/user-attachments/assets/your-image-id-here" width="1000">
</p>

## Features

- Fully automated sorting of multi-material workpieces.  
- Dual operation modes: **Manual** and **Automatic**.  
- **Sequential Function Chart (SFC)**–based task control and **Ladder Logic (LAD)** integration.  
- Fault detection, reset logic, and system status indicators.  
- Modular and reusable PLC function blocks for efficient debugging and expansion.  

## System Architecture

- **PLC Platform:** Siemens S7-1200  
- **Programming Environment:** Siemens TIA Portal (Step 7)  
- **Programming Languages:**  
  - **SFC:** For sequential control of the panel and sorting process.  
  - **LAD:** For integrating FBs and managing system interlocks.  
- **Sensors:** Inductive, capacitive, and optical sensors for part detection.  
- **Actuators:** Conveyor motor, pneumatic cylinders, and sorting gates.  
- **HMI Components:** Start/Stop switches, mode selectors, and indicator lights.  

## Implementation Details

- **Function Block 1 (Control Panel):**  
  Handles manual/auto mode selection, start/stop logic, and system status control.  

- **Function Block 2 (Sorting Task):**  
  Defines the main sorting sequence—detecting workpiece type, activating actuators, and routing items.  

- **Main OB1:**  
  Implemented in **Ladder Logic**, importing the two SFC-based function blocks for modular execution.  

## Results

- Achieved **complete automation** of the sorting station.  
- Improved control structure through **SFC-LAD integration**.  
- Demonstrated proficiency in **industrial automation**, **PLC programming**, and **system design**.  

## Technologies Used

- **Siemens TIA Portal (Step 7)** – PLC programming environment  
- **S7-1200 PLC** – Control hardware  
- **Festo MPS Sorting Station** – Mechatronic system  
- **SFC & LAD** – PLC programming languages  
- **Industrial Sensors & Actuators** – Real-time data acquisition and motion control  

## Documentation
Official reference:  
🔗 [Festo MPS Sorting Station Documentation](https://ip.festo-didactic.com/Infoportal/MPS/SortingStation/EN/index.html)

## Getting Started

If you’d like to explore the logic or replicate the system:

1. Open **Siemens TIA Portal** (vXX or later).  
2. Import the project file containing:  
   - `FB_ControlPanel` (SFC)  
   - `FB_SortingTask` (SFC)  
   - `OB1_Main` (LAD)  
3. Assign I/O according to the MPS station wiring diagram.  
4. Download the project to the **S7-1200 PLC** and start the station in manual or automatic mode.

## 📞 Contact
If you have any questions, feedback, or suggestions regarding this project, feel free to reach out:

- **Name:** Mohammadamin Lari  
- **Email:** [mohammadamin.lari@gmail.com](mailto:mohammadamin.lari@gmail.com)  
- **GitHub:** [AminLari](https://github.com/aminlari)

You are welcome to create issues or pull requests to improve this project. Contributions are highly appreciated!  
