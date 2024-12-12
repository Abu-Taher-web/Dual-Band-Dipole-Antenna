<div align = 'center'>
  <img src="images/dipole_antenna.gif" alt="Description of Image" width="300" style="border: 5px solid black"/>
</div>

# Dual Band Dipole Antenna Design

## Overview

This project focuses on the design, simulation, and analysis of a **Dual Band Dipole Antenna**. The antenna is designed using **CST Studio** and the aim is to study its radiation properties and frequency response by analyzing various antenna parameters. The primary objective of this project is to design a dual band dipole antenna that operates at specific frequencies and meets the required performance criteria.

## Table of Contents

1. [Aim of the Design](#aim-of-the-design)
2. [Theory](#theory)
3. [Input Parameters](#input-parameters)
4. [Calculated Parameters](#calculated-parameters)
5. [Technical Objectives](#technical-objectives)
6. [Design Optimization](#design-optimization)
7. [Output Considerations](#output-considerations)
8. [Design Accuracy](#design-accuracy)
9. [Finally](#finally)
10. [Folder Structure](#folder-structure)

## Aim of the Design

The goal is to design and simulate a basic dual band dipole antenna at a specific frequency and study its radiation properties and frequency response. The design process is carried out using **CST Studio** simulation software.

## Theory

A dipole antenna consists of two identical conductive elements. It operates at the lowest impedance and the voltage and current vary along the radiating section. The antenna is designed to resonate at the desired frequencies.

## Input Parameters

- **Length of the Dipole (L)**: 62.46 cm
- **Radius of the Dipole (R)**: 1.5 cm
- **Frequency of the antenna**: 2.4 GHz
- **Input Impedance**: 73 Ω

The input impedance, radiation intensity, and radiated power are calculated based on the given parameters.

## Calculated Parameters

| Symbol | Value   | Description                 |
|--------|---------|-----------------------------|
| R      | 1.5 cm  | Radius of the Dipole        |
| L      | 62.46 cm| Length of the Dipole        |
| F      | 10      | Feed line of Dipole         |
| Z      | 73 Ω    | Input Impedance of Dipole   |
| f      | 2.4 GHz | Operating Frequency         |

## Technical Objectives

To design a dual band dipole antenna, the following parameters are considered:
- Radiation Pattern
- Frequency Response
- Gain

## Design Optimization

Optimization of the antenna design is performed to ensure that the antenna operates efficiently at the desired frequencies, achieving good performance for the required parameters.

## Output Considerations

- **S-Parameter**: Shows the reflection coefficient and bandwidth of the antenna.
- **Reference Impedance**: The input impedance of the antenna.
- **VSWR**: Voltage Standing Wave Ratio for impedance matching.
- **Gain**: The gain of the antenna in dBi.
- **Directivity**: Directivity of the antenna, showing the focused energy direction.
- **Radiation Patterns**: Both 1-D and 2-D radiation patterns are analyzed to understand the antenna's radiation behavior.

### S-Parameter
The S-parameter of the antenna is shown in the following figure, which indicates the reflection coefficient at the operating frequencies.

![S-parameter](images/s_parameters.png)

### Bandwidth Calculation
From the S-parameter, the bandwidth of the antenna is calculated:
- **BW1** = 0.535 GHz (2.6906 - 2.1556)
- **BW2** = 0.645 GHz (7.7328 - 7.0873)

### Reference Impedance
The input impedance of the dual band dipole antenna is shown below.

![Input Impedance](images/imput_impedence.png)

### VSWR
The Voltage Standing Wave Ratio (VSWR) is an important parameter for impedance matching.

![VSWR](images/voltage_standing_wave_ratio(VSWR).png)

### Gain
The gain of the dual band dipole antenna is calculated as **2.025 dBi**.

![Gain](images/gain_and_directivity.png)

### Directivity
The directivity of the antenna shows how the antenna radiates energy in different directions.

![Directivity](images/gain_and_directivity.png)

### Radiation Patterns
The radiation patterns in both 1-D and 2-D are shown below.

#### 1-D Radiation Pattern
![1D Radiation Pattern](images/1d_radiation_pattern.png)

#### 2-D Radiation Pattern
![2D Radiation Pattern](images/2d_radiation_pattern.png)

## Design Accuracy

The directivity of the dipole antenna achieved by simulation is **2.030 dBi**, which is very close to the calculated value, indicating good design accuracy.

## Finally

- A **Dual Band Dipole Antenna** was successfully designed and simulated.
- All output parameters, including S-parameters, gain, directivity, and radiation patterns, were obtained with maximum accuracy.

## Folder Structure
```
The project folder structure is organized as follows:
Antenna-wifidipole/
├── DC
├── Model
│   ├── 3D
│   ├── ASM
│   ├── CBLS
│   │   └── Harness
│   ├── DS
│   │   ├── Block
│   │   └── Images
│   └── PCBS
│       └── Design
├── ModelCache
├── Result
│   ├── Cache
│   ├── DS
│   │   └── Block
│   ├── Meshfill
│   └── MS
├── SP
├── Temp
├── images
├── presentation
└── source file
```

- **Antenna-wifidipole**: Contains the main project files, including model, results, and design files.
- **images**: Contains images related to the project (S-parameters, radiation patterns, etc.).
- **presentation**: Contains the presentation files for the project.
- **source file**: Contains the source code and configuration files.

## Installation

To run this project, you need **CST Studio** for antenna simulation. Follow the steps below:
1. Open CST Studio.
2. Load the **Model** files from the `Antenna-wifidipole` folder.
3. Run the simulation and analyze the results.

## License

This project is licensed under the MIT License. See the LICENSE file for more information.
