# Bio-PT 🫀
Open Source 3D Bioprinter by | Dr.Islam Salama 
| Linkedin https://www.linkedin.com/in/dr-islam-sa


---

# Bio-PT: Open-Source 3D Bio-Printer

**Bio-PT** is an affordable, open-source 3D bio-printer designed to make bio-printing accessible to students, researchers, and makers worldwide. Built primarily from recycled materials and commonly available components, Bio-PT aims to reduce e-waste and carbon footprint while providing a powerful platform for bio-printing research and prototyping.

The Bio-PT operates using a modified version of Marlin firmware (1.1.9), termed **Bio-Marlin**, which enables the printer to work efficiently with an indirect syringe pump. The design uses CD-ROM drive motors, a 3D-printed frame, and an indirect extrusion system to minimize costs and weight on the X and Z axes.

## Table of Contents
1. [Features](#features)
2. [Hardware Overview](#hardware-overview)
3. [Firmware - Bio-Marlin](#firmware---bio-marlin)
4. [Bill of Materials](#bill-of-materials)
5. [Assembly Instructions](#assembly-instructions)
6. [Setup and Usage](#setup-and-usage)
7. [Recommended Controller Boards](#recommended-controller-boards)
8. [Environmental Impact](#environmental-impact)
9. [FAQ](#faq)
10. [Contributing](#contributing)
11. [License](#license)

---

## Features

- **Affordable**: Bio-PT is designed with low-cost components, making bio-printing accessible for academic and hobbyist purposes.
- **Sustainable Design**: The frame and majority of components are 3D-printed or sourced from recycled materials, reducing e-waste and overall cost.
- **Indirect Syringe Pump Extruder**: Lightweight, indirect extrusion reduces load on the X and Z axes, improving performance.
- **Modified Firmware**: Bio-PT runs on Bio-Marlin, a version of Marlin firmware modified to accommodate bio-printing needs.
- **Compatibility**: Works with RAMPS boards and MKS boards with built-in IC drivers.

---

## Hardware Overview

### 3D Printed Frame
- Designed for FDM 3D printers.
- Parts can be assembled with M3 x 6mm fasteners, which are easy to source globally.

### Motion System
- Utilizes CD-ROM drive motors for X, Y, and Z movement, which greatly reduces the cost of traditional motors.
- Supports smooth movement and controlled extrusion.

### Extrusion Mechanism
- Indirect syringe pump serves as the extruder, helping to maintain minimal weight on the moving axes.
- Ideal for printing bio-materials or experimental composites.

---

## Firmware - Bio-Marlin

Bio-PT operates using **Bio-Marlin**, a customized firmware derived from Marlin 1.1.9. Bio-Marlin has been tailored specifically for bio-printing by incorporating features to support indirect syringe extrusion and eliminating heat-related functionalities to match the unique needs of bio-materials.

- **Current Version**: Beta
- **Modifications Include**:
  - Disabled heating elements to support room-temperature extrusion.
  - Customized extruder settings to allow fine-tuning of extrusion for bio-materials.
  - Reduced footprint on processing to work seamlessly with lower-cost boards.

You can download Bio-Marlin from the [Firmware](#) folder in this repository : [Bio-Marlin V1.2 firmware](https://github.com/dr-islam-sa/Bio-Marline) — a modified version of Marlin tailored for bioprinting applications. Bio-Marlin focuses on enhanced control for bio-inks and optimized settings for 3D bioprinting needs.


---

## Bill of Materials

| Part                  | Quantity | Notes                                          |
|-----------------------|----------|------------------------------------------------|
| 3D Printed Frame      | 1 set    | All parts are printable using standard FDM printer |
| CD-ROM Drive Motors   | 3        | Used for X, Y, and Z axes                      |
| M3 x 6mm Fasteners    | 40       | Available from any hardware store              |
| M4 x 4mm Fasteners    | 5        | Available from any hardware store              |
| M3       Washers      | 15       | Available from any hardware store              |
| RAMPS or MKS Board    | 1        | Open-source controller board                   |
| S.Pump Lead Screw M6 X16cm | 1        | Indirect extruder system                       |

---

## Assembly Instructions

1. **3D Print Frame Components**:
   - Print all frame parts using PLA or ABS (or other FDM-compatible materials) and assemble using M3 x 6mm fasteners.
  
2. **Install Motors and Drive Components**:
   - Secure CD-ROM motors for X, Y, and Z axes using the pre-designed mounting areas on the frame.
  
3. **Attach Syringe Pump Extruder**:
   - Set up the syringe pump as the extruder mechanism, ensuring it is positioned to reduce load on the X and Z axes.
  
4. **Connect Electronics**:
   - Use the RAMPS or MKS board to connect motors and extruder. Follow the wiring diagram provided in the `Documentation` folder.

---

## Setup and Usage

### Initial Setup
1. **Upload Bio-Marlin Firmware**:
   - Compile and upload the customized Bio-Marlin firmware to your controller board.
  
2. **Calibration**:
   - Calibrate the printer for X, Y, and Z movement and set the extrusion parameters.
  
3. **Syringe Loading**:
   - Carefully load your bio-material into the syringe. Ensure it is compatible with the printer specifications.

### Printing
1. Load your model in your preferred slicer software.
2. Export the G-code and run it on Bio-PT.
3. Monitor the print to ensure proper extrusion and movement.

---

## Recommended Controller Boards

### RAMPS
An open-source, affordable option that works well with Bio-Marlin.

### MKS Boards
- The MKS board with built-in IC drivers is highly recommended for stability and ease of setup.

---

## Environmental Impact

Bio-PT is designed with sustainability in mind:
- **Recycled Materials**: Using recycled parts, especially the CD-ROM motors, minimizes environmental impact.
- **Carbon Footprint Reduction**: By choosing 3D-printed parts and recycled components, Bio-PT contributes to a reduced carbon footprint in comparison to conventional manufacturing.
- **Low-Energy Consumption**: The choice of lightweight materials and efficient motors keeps the printer’s power consumption low.

---

## FAQ

**Q1: What materials can Bio-PT print?**  
Bio-PT is primarily designed for bio-materials that can be extruded from a syringe, such as gels, pastes, and soft polymers. Avoid using traditional filament-based materials.

**Q2: Is the firmware fully stable?**  
Bio-Marlin is currently in beta, so some features are still being optimized for bio-printing.

**Q3: How can I get replacement parts?**  
Most parts are easily replaceable with standard hardware. The STL files for 3D printing the frame are available in the repository.

---

## Contributing

Bio-PT is an open-source project, and contributions are welcome! If you want to contribute, please:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Submit a pull request with a detailed description of your changes.

For major changes, please open an issue to discuss your idea first.

---

## License

This project is licensed under the [GNU 3.0 License](LICENSE), which allows for personal and commercial modification and distribution as long as the original author is credited.

Here’s the GNU General Public License v3.0 text, which you can include in your GitHub project:

---

# GNU GENERAL PUBLIC LICENSE  
Version 3, 29 June 2007

Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org>  
Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.


## TERMS AND CONDITIONS

### 0. Definitions.

“This License” refers to version 3 of the GNU General Public License.

“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.

“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you.” “Licensees” and “recipients” may be individuals or organizations.

To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.

A “covered work” means either the unmodified Program or a work based on the Program.

To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.

To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.

An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.

(Sections 1 through 15 continue the terms in detail. If you want the full text, it is available [here](https://www.gnu.org/licenses/gpl-3.0.txt).)

---

To apply this license, include this in your project’s documentation or source code files:

```
Bio-PT - An open-source 3D Bio-printer

Copyright (C) <2024> <Dr.Islam Salama>

This project is free opensource: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License..

This project is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this project. If not, see <https://www.gnu.org/licenses/>.
```
---
