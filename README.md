# Festo MPS Sorting Station Automation

## Overview
Automation of the **Festo MPS Sorting Station** using **Siemens TIA Portal** and **SIMATIC S7-1500 PLC**.  
The system classifies workpieces by **material** and **color**, using a sequence of sensor readings and actuator controls coordinated through a modular PLC program.

<p> 
  <img src="https://github.com/user-attachments/assets/1504566d-5cd9-44fc-9b20-0cf1b52f0b12" width="1000">
</p>

## Features

- Fully automated sorting of multi-material workpieces.  
- Dual operation modes: **Manual** and **Automatic**.  
- **Sequential Function Chart (SFC)**–based task control and **Ladder Logic (LAD)** integration.  
- Fault detection, reset logic, and system status indicators.  
- Modular and reusable PLC function blocks for efficient debugging and expansion.  

## System Architecture

- **PLC Platform:** Siemens S7-1500  
- **Programming Environment:** Siemens TIA Portal (Step 7)  
- **Programming Languages:**  
  - **SFC:** For sequential control of the MPS station control panel and sorting process.  
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

## Documentation
Official reference:  
🔗 [Festo MPS Sorting Station Documentation](https://ip.festo-didactic.com/Infoportal/MPS/SortingStation/EN/index.html)

## Getting Started

If you’d like to explore the logic or replicate the system:

1. Open **Siemens TIA Portal** (vXX or later).  
2. Import the `.zap16` project file containing:  
   - `FB_ControlPanel` (SFC)  
   - `FB_SortingTask` (SFC)  
   - `OB1_Main` (LAD)  
3. Assign I/O according to the MPS station wiring diagram.  
4. Download the project to the **S7-1500 PLC** and start the station in manual or automatic mode.

## Program Structure
**1. Main OB1**
<p> 
  <img src="https://github.com/user-attachments/assets/f1a9e919-a818-422b-9007-581016008d4c" width="400">
</p>

**2. Control Panel**
<p>
<img src="https://github.com/user-attachments/assets/f8c3f649-97f0-4f1a-9367-b7a8e98c635f" width="400">
</p>

**3. Sorting Logic**
<p>
<img src="https://github.com/user-attachments/assets/b08addd7-8b1f-4399-b9c7-217299ea41e1" width="400">
</p>

**4. HMI**
<p>
<img src="https://github.com/user-attachments/assets/def34ab6-4919-413f-9337-018646b86d37" width="400">
</p>

## 📞 Contact
If you have any questions, feedback, or suggestions regarding this project, feel free to reach out:

- **Name:** Mark Lari  
- **Email:** [mark.lari.work@gmail.com](mailto:mark.lari.work@gmail.com)  
- **GitHub:** [AminLari](https://github.com/aminlari)

You are welcome to create issues or pull requests to improve this project. Contributions are highly appreciated!  
