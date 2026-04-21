# Byzantine-Resilient WiFi HaLow Fingerprinting Dataset

This repository contains the experimental datasets used in the study: *"Experimental Impact Analysis of Byzantine Attacks on WiFi HaLow Fingerprinting-Based Positioning"*.

## Hardware Configuration
The measurement campaign was conducted using an IoT infrastructure based on the following components:

* **Nodes:** 5x Raspberry Pi 4 Model B.
* **Interfaces:** ALFA AHPI7292S WiFi HaLow modules (Newracom NRC7292 chipset).
* **Configuration:** Open network mode, EU regulatory region.

## Research Goals
This work aims to assess the reliability of localization data (RSSI/Fingerprinting) in long-range IoT networks. Specifically, the research addresses the following objectives:

1. **Impact Analysis:** Quantifying how Byzantine attacks—where compromised nodes inject false signal data—degrade localization accuracy.
2. **Mitigation:** Establishing a "clean" baseline to develop and evaluate detection algorithms for malicious anchor nodes.
3. **Validation:** Demonstrating system performance in real-world outdoor scenarios subject to fading and shadowing phenomena typical of sub-GHz communication bands.

## Repository Structure
The data is organized by measurement campaign:

- **`/Data/ScenarioLinear`**: Dataset for linear propagation analysis (Clean Baseline). [View details](./Data/ScenarioLinear/README.md)
- **`/Data/Fingerprinting`**: Dataset for radio fingerprinting-based localization. [View details](./Data/ScenarioFingerprinting/README.md)

## License and Citation
This dataset is distributed under the Creative Commons Attribution 4.0 International License.
If you use this dataset in your research, please cite our paper:

```bibtex
@article{PeCuPiMa26,
  author = {Pettorru, Giovanni and Curridori, Marta and Pilloni, Virginia and Martalò, Marco},
  title = {Experimental Impact Analysis of Byzantine Attacks on WiFi HaLow Fingerprinting-Based Positioning},
  journal = {To be defined/Insert Conference or Journal Name},
  year = {2026}
}