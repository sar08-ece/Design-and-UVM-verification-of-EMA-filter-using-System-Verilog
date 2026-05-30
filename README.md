# Adaptive EMA Low Pass Filter using SystemVerilog and UVM

## Project Description

This project implements an Adaptive Exponential Moving Average (EMA) Low Pass Filter on an Intel MAX10 FPGA using SystemVerilog. The filter is designed to reduce noise from sampled audio signals while allowing dynamic adjustment of the filtering strength through switch-controlled parameters.

Audio samples are generated and processed in MATLAB, converted into HEX/MIF files, loaded into FPGA memory, filtered using the EMA algorithm, and stored back for analysis. The design is verified using a UVM-based self-checking testbench.

## Features

* EMA-based Low Pass Filter implementation
* Dynamic filter strength selection
* FPGA memory-based signal processing
* MATLAB preprocessing and HEX/MIF generation
* SystemVerilog RTL design
* UVM verification environment
* Self-checking scoreboard
* Multiple randomized test cases
* PASS/FAIL based functional validation

## Tools and Technologies

* SystemVerilog
* UVM (Universal Verification Methodology)
* MATLAB
* Intel Quartus Prime
* EDA Playground
* Intel MAX10 FPGA

## Verification

A UVM testbench was developed consisting of:

* Sequence
* Driver
* Monitor
* Agent
* Environment
* Scoreboard

The scoreboard compares DUT outputs against a reference EMA model and reports PASS/FAIL results automatically.

## Results

* Successful FPGA implementation
* Correct filtering operation verified
* UVM verification completed with zero functional mismatches
* Dynamic switching between multiple filter strengths demonstrated

## Future Enhancements

* Real-time ADC integration
* Functional coverage collection
* SystemVerilog Assertions (SVA)
* FIR filter implementation and comparison
* Real-time audio playback through DAC/Codec
* Adaptive noise-level-based filter selection
