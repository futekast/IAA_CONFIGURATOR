# IAA Series Gain & Shunt Configurator

A lightweight desktop GUI tool for calculating gain and shunt (shunt-calibration) settings for the FUTEK IAA Series signal conditioners, with a clean and user-friendly interface.

Designed for engineers, technicians, and production staff configuring IAA100, IAA200, and IAA300 instrumentation amplifiers.

---

## Features

- Supports the IAA100, IAA200, and IAA300 series
- Recommends the best DIP-switch gain configuration for your target output
- Lists all other valid gain configurations, not just one answer
- Voltage-output and current-output device support
- Shunt-calibration network calculator (shunt across the bridge leg)
- Live DIP-switch diagram that matches each configuration
- Input preview and validation as you type
- Lightweight standalone executable (no installation required)

---

## Supported Devices

### IAA100

- IAA100 / FSH04939
- IAA100 / FSH04935
- IAA100 / FSH04461
- IAA100 / FSH03863

### IAA200

- IAA200 / FSH03864
- IAA200 / FSH04804
- IAA200 / FSH04936
- IAA200 / FSH04940
- IAA200 / QSH02442

### IAA300

- IAA300 / FSH03931
- IAA300 / FSH04875

---

## How It Works

### Gain Tab

Enter the sensor rated output (mV/V), the excitation voltage, and your target output. The tool computes the required gain and recommends the DIP-switch setting that comes closest, along with a table of every other valid configuration.

### Shunt Tab

Enter the bridge resistance and the selected gain DIP code to calculate the shunt-calibration output across the bridge leg. Output is shown in volts, or in milliamps for current-output devices.

### Configuration Tab (IAA200)

Walk through the IAA200 calibration steps: set the Gain and Shunt DIP switches per the configuration and verify they all match exactly. Then adjust the Offset potentiometer with no sensor load, press and HOLD the Shunt button, and adjust the Span potentiometer to the configuration target.

---

## Usage

1. Select the Model and Item (FSH/QSH) from the Product bar
2. Choose the Gain, Shunt, or Configuration tab
3. Enter your inputs
4. Read the recommended setting and the DIP-switch diagram
5. Review the table of other valid configurations if needed

---

## Notes

- This tool performs calculation and configuration guidance only; it does not communicate with hardware
- DIP numbering is DIP1 … DIP8, left to right
- Values follow each device's published electrical profile

---

## License

This repository contains the GUI tool only.

Underlying electrical profiles and algorithm implementations may be proprietary and are not distributed as source code in this repository.
