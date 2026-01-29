# PerfectPixel ComfyUI Node

This document describes the usage of the **Perfect Pixel (Grid Restore)** node in ComfyUI.

> For Chinese documentation, see: 
> https://github.com/TobyKSKGD/perfectPixel-ComfyUI#

## Node Parameters

![example](../../images/comfyui.png)

The **Perfect Pixel (Grid Restore)** node provides the following configurable parameters:

- **sampling**
  Sampling method used when restoring pixel grids.

- **export_scale**
  Scaling factor applied to the output image.

- **backend**
  Backend implementation to use:
  - **Auto**: Automatically selects the available backend
  - **OpenCV Backend**: Uses OpenCV for better performance
  - **Lightweight Backend**: NumPy-only implementation without OpenCV

## Getting Started

### One-Click Installation

If Git is already installed, run the following command inside `ComfyUI/custom_nodes` and then restart ComfyUI:

```bash
git clone https://github.com/TobyKSKGD/perfectPixel-ComfyUI.git
```

### Manual Installation

Download this repository, then copy the entire `./integrations/comfyui/perfectPixel-ComfyUI` folder into `ComfyUI/custom_nodes`.
Restart ComfyUI after copying.

After restarting, search for **Perfect Pixel (Grid Restore)** in the node search panel on the left to find the node.
The node is located at: `Image → Post Processing → Perfect Pixel (Grid Restore)`

## Dependencies

This node requires the following dependencies:

- `numpy`
- `opencv-python` (optional, required for OpenCV backend)

Install dependencies with:

```bash
pip install numpy
pip install opencv-python
