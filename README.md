# KiCad Random Components Library

A collection of custom KiCad footprints and symbols for components that aren't readily available in standard libraries but have proven useful in various projects.

## Purpose

This repository aims to provide ready-to-use KiCad footprints and symbols for components that may be difficult to find in standard libraries. Hopefully this saves someone else some time.

## Currently Available Components

### 1. MSK12C02G15-B Slide Switch (HanElectricity)

A small slide switch manufactured by HanElectricity Co., Ltd. 

- Operating voltage: DC 12V, 0.1A
- Insulation resistance: >100MΩ
- Contact resistance: <50MΩ
- Operating force: 160gf±50gf
- High temperature resistance: 260°C
- Available in different heights and colours

### 2. eAce11 Embedded PLC Board (Velocio Networks)

This is a footprint and symbol for integrating the entire eAce11 PLC board into custom PCB designs. Rather than representing the individual components on the PLC itself, this allows you to incorporate the complete board as a module in your larger PCB projects.

The eAce11 is an embedded version of Velocio's Ace11 PLC, designed for integration into custom motherboards. It offers powerful automation capabilities in a small form factor.

- 6 Digital Inputs (3-30VDC, high-speed pulse counting capability)
- 6 Digital Outputs (sinking transistor outputs with step/direction motion control)
- USB programming port with Modbus RTU slave capability
- PWM capability on all outputs
- Small footprint (2.5"H x 2.5"W x 0.5" deep)
- Programmed using Velocio's vBuilder software

### 3. EasyDriver v4.4 Stepper Motor Driver Board

This footprint and symbol is for integrating the entire EasyDriver board into your PCB designs, not for the individual components on the board itself. This allows you to design PCBs that incorporate the EasyDriver as a complete module.

The EasyDriver is a simple-to-use stepper motor driver board compatible with motors operating at 7-30V. It can drive bi-polar motors with 4, 6, or 8 wires.

- Motor supply voltage: 6-30V
- Motor coil current: up to 750mA per phase
- Logic supply voltage: 5V (on-board regulator provides 5V out)
- Step frequency: up to 500kHz
- Step modes: full, half, quarter, eighth
- Control inputs: Step, Direction, MS1, MS2, Enable, Reset, Sleep

## Usage

1. Clone or download this repository
2. In KiCad, add this library to your project:
   - For symbols: Preferences > Manage Symbol Libraries > Add
   - For footprints: Preferences > Manage Footprint Libraries > Add
3. Browse and use the components in your schematics and PCB layouts

## Usage Examples

### EasyDriver and eAce11 PLC Integration

These footprints are particularly useful for projects where you need to integrate pre-built modules into a custom PCB. For example:

- A custom control board that incorporates both the eAce11 PLC for automation logic and an EasyDriver for motor control
- PCBs designed to serve as carrier boards or backplanes for these modules
- Projects requiring both processing capability and motor control in a compact form factor

## Contributing

Contributions are welcome! If you have created footprints or symbols for components not widely available, consider adding them to this repository. Please ensure that:

1. Your submissions include both symbol and footprint where applicable
2. You provide basic documentation about the component
3. The footprints are validated (if possible)
4. You include a reference to the component datasheet or specifications

## License

This library is released under the [GLP-3.0 license](LICENSE.md).

## Acknowledgments

- Thanks to the KiCad team for providing an excellent open-source EDA software
- Component manufacturers for their documentation and specifications
