# SW-YOLO

## Model Configuration Instructions

- All custom models are located under `cfg/models/mycfg/`, defined by scale, backbone, head, and other structures.
- Modify the YAML file to quickly switch network depth, width, and module type.

---

## New Module Introduction

- **SWBlock_spatial_attention**: CSP core, integrates spatial attention.
- **SWBlock_channel_attention**: Integrates channel attention branch.
- **Conv**: Automatically selects BatchNorm or LayerNorm based on grouping.
