# Methodology – How Red Canary Detects and Counts Threats

## Data Collection
Red Canary processes:
- **1 PB/day** of endpoint telemetry
- **14 million investigative leads**
- **33,000+ confirmed threats**

Telemetry sources include:
- Process execution
- Command-line arguments
- Network connections
- File modifications
- Parent-child process relationships

---

## Detection Pipeline
1. Telemetry enters the analytics engine.
2. ~3,000 detection analytics evaluate the data.
3. If telemetry matches analytic logic → an **event** is generated.
4. A detection engineer reviews the event.
5. If malicious/suspicious → it becomes a **confirmed threat**.
6. The confirmed threat inherits the MITRE ATT&CK techniques mapped to the analytic.

---

## Technique Counting Method
For each malicious/suspicious detection:
- Every technique mapped to contributing analytics is incremented.
- Reinfection on the same host counts as a new detection.
- This emphasizes techniques commonly reused across environments (e.g., lateral movement).

### Parent vs Sub-Techniques
- If a sub-technique accounts for **≥20%** of detections for a technique → analyze the sub-technique.
- If not → analyze the parent technique.

---

## Threat Counting Method
Threats (malware, tools, groups) are counted by:
- **Unique customer environments**, not number of detections.

Reason:
- Prevent ransomware and lateral movement tools (e.g., Cobalt Strike) from dominating the statistics.

---

## Limitations
- Visibility is primarily **EDR-based**, so:
  - Email-only threats may be underrepresented.
  - Network-only threats may be underrepresented.
- Some threats may be underreported if not detected.
- Defenders should build their own threat model using:
  - This report
  - Other vendor reports
  - Internal telemetry

---

## Key Takeaways
- The methodology prioritizes **behavioral detection**.
- Technique counts reflect what defenders are most likely to encounter.
- Threat counts reflect how widespread a threat is across organizations.
- Understanding the methodology helps SOC analysts interpret the data correctly.

