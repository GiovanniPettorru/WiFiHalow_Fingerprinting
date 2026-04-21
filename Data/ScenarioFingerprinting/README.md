# Dataset: Radio Fingerprinting

## Experimental Scenario
This dataset was collected at the CUS sports citadel in Cagliari, Italy. The experiment involved placing the Access Point (AP) at 9 different predefined positions within the sports field while the client nodes remained associated. The primary objective is to correlate physical and MAC layer metrics with specific spatial coordinates for radio fingerprinting-based localization techniques.

<figure>
  <img src="img/FingerprintingScenario.png" alt="Fingerprinting scenario setup" width="70%">
  <figcaption>Figure 1: Experimental setup for WiFi HaLow fingerprinting measurements.</figcaption>
</figure>

## Data Acquisition
- **Sampling Frequency:** 1 Hz (1 measurement per second).
- **Duration:** 10 minutes of continuous data collection for each of the 9 positions.
- **Data Cleaning:** Outliers removed using a 1st–99th percentile filter.
- **Files:** `Position_1.csv` to `Position_9.csv` contain the post-processed radio metrics.

## Data Structure
The CSV files use a semicolon (`;`) as a delimiter. Each record contains the following metrics collected from 4 different Access Points (AP):

| Column Name | Description |
| :--- | :--- |
| `position_id` | Identifier of the Access Point position (1 to 9) |
| `RSSI_APx` | Received Signal Strength Indicator for AP *x* (dBm) |
| `SNR_APx` | Signal-to-Noise Ratio for AP *x* (dB) |
| `MCS_APx` | Modulation and Coding Scheme for AP *x* |

*Note: The metrics (`RSSI`, `SNR`, `MCS`) are provided for 4 distinct Access Points (AP1 to AP4).*

## Technical Details
- **Devices:** Raspberry Pi 4 Model B equipped with ALFA AHPI7292S (Newracom NRC7292 chipset) WiFi HaLow modules.
- **Configuration:** Open network mode, EU regulatory region.