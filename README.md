# Llama 70B Inference on Dual GPUs

An experiment exploring quantized Llama 70B inference using
llama.cpp with CUDA GPU offloading in a dual-GPU environment.

## Overview

This project demonstrates the configuration and execution of
a quantized Llama 70B model using GPU layer offloading,
context-length configuration, and batch-size settings.

## Technical Details

- Model: Llama 70B quantized GGUF
- Framework: llama-cpp-python / llama.cpp
- GPU configuration: Dual-GPU CUDA offloading
- Context length: 2048 tokens
- Batch size: 512
- GPU-offloaded layers: 60/81 (as shown in the execution logs)

## Results

The notebook includes model-loading logs, GPU memory
information, inference performance measurements, and
a generated response.

## Limitations

The experiment uses partial GPU offloading, with some
model resources mapped to CPU memory. Performance and
memory usage depend on the hardware and configuration.
