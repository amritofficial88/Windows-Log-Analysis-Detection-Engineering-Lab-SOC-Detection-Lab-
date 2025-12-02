# SOC Detection Lab

This repo contains hands-on blue team projects focused on building detections, analyzing Windows logs, and simulating adversary techniques using Splunk, Sigma, and MITRE ATT&CK.

## Detection Use Cases

| Detection Name                  | Tool     | Log Type               | MITRE Technique     |
|--------------------------------|----------|------------------------|---------------------|
| Suspicious PowerShell Use      | Splunk   | WinEventLog:Security   | T1059.001           |
| Multiple Failed Logins (4625)  | Splunk   | Security.evtx          | T1110.001           |
| Encoded PowerShell Command     | Sigma    | Sysmon + EVTX          | T1059, T1140        |

## Contents

- `detections/` → SPL and Sigma rules
- `logs/` → Sample `.evtx` logs from public data sets
- `dashboards/` → Exported JSON dashboards from Splunk
- `screenshots/` → Visuals from successful detections
- `playbooks/` → Markdown guides for detection and validation

## Tools Used

- Splunk Enterprise (Free)
- Sigma (with sigmac converter)
- MITRE ATT&CK Navigator
- EVTX Sample Logs (from public GitHub repos)

## What I Learned

- How to detect real-world TTPs from public log data
- How to convert threat intel into detections
- How to tune false positives and write meaningful alerts

## Sample Log Sources

- [EVTX-ATTACK-SAMPLES](https://github.com/sbousseaden/EVTX-ATTACK-SAMPLES)
- [Hayabusa Sample EVTX](https://github.com/Yamato-Security/hayabusa-sample-evtx)

