# FPGA-accelerated-ML-inference-accelerator
implementing a custom inference accelerator in the FPGA fabric



Overview

This project explores hardware-software co-design by implementing a custom neural network inference accelerator in Verilog, deployed on the programmable logic (PL) of a Zynq-7000 SoC, and controlled via Python through PYNQ running on the onboard ARM Cortex-A9 (PS).

A classification model is trained on GPU (PyTorch), quantized to int8 fixed-point, and its inference computation is offloaded to a custom multiply-accumulate (MAC) based accelerator in the FPGA fabric — with the goal of comparing FPGA-accelerated inference against CPU-only and GPU baselines for latency and resource efficiency.
