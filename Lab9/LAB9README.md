# Lab 9: YANG to UML Diagram

This lab demonstrates how to use `pyang` and `plantuml` on Ubuntu WSL to convert a YANG model into its YIN representation and a UML diagram. The final output includes a `.png` UML class diagram generated from a `.yang` file.

## Lab Summary

- The YANG module describes a simple intrusion detection system.
- The YIN file is the XML-based version of the YANG.
- The UML file is generated using `pyang` and visualized using PlantUML.
- All tasks were completed inside WSL Ubuntu using a virtual Python environment to bypass system-level pip restrictions.

## Final UML Diagram

![uml](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/intrusiondetection.png?raw=true)

This is the final UML diagram generated from the YANG file. It visually represents the module, containers, lists, leaf nodes, RPCs, and notifications.

## Screenshots

### 1. WSL and Ubuntu Installation
![wslinstall](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%231.png?raw=true)

### 2. apt and pip Setup
![aptpip](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/Lab9%232.png?raw=true)

### 3. pip install for pyang and plantuml
![pipinstall](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%233.png?raw=true)

### 4. GitHub Clone and File Setup
![clone](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%234.png?raw=true)

### 5. Converting YANG to YIN and UML
![pyang](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%235.png?raw=true)

### 6. Fixing missing Python modules
![fixdeps](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%236.png?raw=true)

### 7. Successful Diagram Generation
![success](https://github.com/acana68/Engineering-Design-VI/blob/main/lab9/lab9%237.png?raw=true)

## Files Created

- `intrusiondetection.yang` – Original model file.
- `intrusiondetection.yin` – XML-based YIN version.
- `intrusiondetection.uml` – UML source file.
- `intrusiondetection.png` – Final UML diagram image.

