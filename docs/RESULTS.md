# Preliminary Results

The values in this preview are taken from the current manuscript experiments. They are provided to document the repository release and may be expanded with additional seeds and test protocols in a later version.

## Evaluation Protocols

Two SpaceNet 6 protocols are reported separately:

1. **Clean-only training:** the model is trained and evaluated using clean optical observations.
2. **Mixed-degradation training:** the training index contains clean, light, medium, and heavy optical conditions; the same checkpoint is evaluated across the four conditions.

Both protocols use aligned SAR observations and unchanged building labels. Foreground-building IoU is reported as a percentage.

## CIRRUS-Net Results

| Training protocol | Clean | Light | Medium | Heavy | Clean-to-Heavy retention |
|---|---:|---:|---:|---:|---:|
| Clean-only training | **83.50** | - | - | - | - |
| Mixed-degradation training | 81.24 | 80.82 | 79.86 | **72.18** | **88.84** |

Under the matched mixed-degradation protocol, CIRRUS-Net exceeds ASANet by 3.84 percentage points under heavy degradation. The corresponding heavy-condition IoU values are 72.18% for CIRRUS-Net and 68.34% for ASANet.

## Cross-Region Transfer

A dual-polarization adaptation using Sentinel-2 RGB and Sentinel-1 VV/VH observations achieves **76.52% IoU** on the Global-S1S2-WorldCover-BuiltUp-10K experiment. This setting evaluates 10 m built-up areas rather than individual high-resolution building footprints and does not instantiate the complete four-polarization degradation-supervised system.

## Robustness Trend

![Cloud-fog robustness](../assets/results/cloud_fog_robustness.png)

[PDF version](../assets/results/cloud_fog_robustness.pdf)

The robustness curve compares models trained under the same mixed-degradation protocol. CIRRUS-Net retains 88.84% of its clean-condition IoU under heavy degradation, compared with 87.91% for ASANet, 86.04% for MSSNet, and 82.52% for MCANet.

## Qualitative Results

### Clean observations

![Clean qualitative comparison](../assets/results/spacenet_clean_qualitative.png)

[PDF version](../assets/results/spacenet_clean_qualitative.pdf)

### Heavy cloud-fog degradation

![Heavy-degradation qualitative comparison](../assets/results/spacenet_degraded_qualitative.png)

[PDF version](../assets/results/spacenet_degraded_qualitative.pdf)

These examples are included to illustrate characteristic segmentation behavior. Aggregate metrics, rather than selected samples, remain the basis for quantitative conclusions.

