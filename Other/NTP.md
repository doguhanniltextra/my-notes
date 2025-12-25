[[ISP]]

NTP is designed to synchronize the clock of computers over a network. While it seems basic, it is the foundation of Distributed Systems Consistency.

- **Log Correlation:** If your on-premise **API Gateway** has a clock 5 seconds ahead of your **ECS Cloud Provider**, you cannot accurately reconstruct the timeline of a single request.
- **Security & Tokens:** JWT tokens and mTLS certificates rely on expiration times. If clocks are out of sync (**Clock Skew**), valid tokens from the Cloud may be rejected by the On-Premise system.
- **Data Integrity:** **Agent 2** tags IoT data with a timestamp. Without NTP, your time-series analysis in the Cloud will show events happening in the wrong order.
### How It Works: The Stratum Model

NTP uses a hierarchical system of time sources:
- **Stratum 0:** Atomic clocks or GPS clocks (High precision).
- **Stratum 1:** Servers directly connected to Stratum 0 devices.
- **Stratum 2:** Servers that synchronize with Stratum 1 (Common for corporate NTP servers).