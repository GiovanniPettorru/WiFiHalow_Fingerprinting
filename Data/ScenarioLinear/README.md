# Dataset: Linear Propagation Analysis

## Experimental Scenario
This dataset was collected at the CUS sports citadel in Cagliari, Italy, in an outdoor environment. The target node remained stationary while the anchor was moved along a straight line at incremental distances (from 5m to 40m). This setup allows for the characterization of RSSI behavior in Line of Sight (LOS) conditions.

<figure>
  <img src="img/LinearScenario.png" alt="Linear scenario setup" width="75%">
  <figcaption>Figure 1: Experimental setup for linear propagation measurements.</figcaption>
</figure>

## Technical Details
- **Devices:** Raspberry Pi 4 Model B equipped with ALFA AHPI7292S (Newracom NRC7292 chipset) WiFi HaLow modules.
- **Configuration:** Line of Sight (LOS), EU regulatory region.
- **Data Cleaning:** Outliers removed using a 1st–99th percentile filter.
- **Files:** `Linear.csv` and `Linear.xlsx` contain RSSI measurements (in dBm).

## Data Structure
The `Linear.csv` file uses a semicolon (`;`) as a delimiter. Each column represents a specific measurement distance:

| Column | Description |
| :--- | :--- |
| `d5` - `d40` | RSSI value (dBm) measured at the corresponding distance (e.g., `d5` = 5 meters). |