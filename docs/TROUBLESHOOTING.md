# Troubleshooting — IoTPredictiveMaintenanceSystem

| Symptom | Check |
|---|---|
| No vibration proxy | Verify sensor power, grounds, pin table, voltage limits, and module orientation. |
| Invalid sample | Check 0–2048 ADC RMS counts range and sensor calibration. |
| Wi-Fi disconnected | Check SSID, 2.4 GHz coverage, and local network policy. |
| MQTT disconnected | Check broker DNS, port 8883, CA PEM, device credentials, and publish ACL. |
| Unexpected alert | Inspect raw vibration proxy and six-sample vibration forecast; calibrate the threshold in `logic.h`. |
| Build failure | Confirm PlatformIO is installed and dependency downloads are permitted. |

EWMA trend projects vibration six samples ahead; no trained failure predictor or remaining-life estimate is claimed.
