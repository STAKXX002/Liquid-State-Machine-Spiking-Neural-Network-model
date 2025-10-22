# Liquid State Machine (LSM) - MNIST to Vivado

This project implements a Liquid State Machine (LSM) Spiking Neural Network trained on the MNIST dataset. 
The trained model is exported to quantized `.mem` files that can be used in Vivado or Verilog simulations.

## Features
- Implements LIF-based Spiking Neural Network
- Ridge regression readout layer
- Exports `.mem` files for FPGA use
- Includes visualizations of reservoir activity

## Requirements
Install the following Python packages before running the notebook:

```
pip install numpy scipy scikit-learn matplotlib
```

## Files
- `LSM_MNIST_CPU_Vivado.ipynb` - Main notebook for training and exporting data
- `Win_q.npz`, `W_q.npz`, `Wout_q.npz` - Quantized weights
- `.mem` files - Exported weights for HDL simulation
- `requirements.txt` - List of dependencies

## Usage
1. Run the notebook to train the LSM and generate `.mem` files.
2. Import the `.mem` files into your Vivado project using `$readmemh`.

## License
MIT License
