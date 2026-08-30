# Degradation Sequence Preview

This directory contains one SpaceNet 6 optical patch rendered at four degradation levels.

| File | Condition | Mean effective alpha | Mean target reliability |
|---|---|---:|---:|
| `clean.png` | Clean | 0.0000 | 1.0000 |
| `light.png` | Light | 0.0962 | 0.9038 |
| `medium.png` | Medium | 0.2277 | 0.7723 |
| `heavy.png` | Heavy | 0.6569 | 0.3431 |

The underlying patch identifier is `tile_5989_y0388_x0256`. The numerical generation metadata are stored in [`metadata.json`](metadata.json).

Only the optical observation is degraded. The aligned SAR observation and building label are unchanged.

## Provenance and Usage Notice

- The clean optical patch is derived from the SpaceNet 6 Expanded Dataset, which is licensed by the SpaceNet Partners under CC BY-SA 4.0.
- The cloud appearance and cloud-mask information used by the degradation compositor originate from HRC_WHU. The HRC_WHU provider states that the dataset is shared for academic purposes only.
- No original HRC_WHU cloud image or annotation is distributed in this directory.
- These four preview files are provided only for academic inspection of the degradation protocol. They are not covered by any future source-code license for CIRRUS-Net.

See [`docs/DATA_SOURCES.md`](../../docs/DATA_SOURCES.md) for full citations and upstream terms.

