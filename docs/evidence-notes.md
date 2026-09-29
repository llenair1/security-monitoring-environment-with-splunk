# Evidence notes

The source is my 2024 **Defensive Security Project** presentation, a 35-slide team deliverable for the UC Berkeley cybersecurity bootcamp. Its title slide names me and four classmates. The scenario describes a fictional Virtual Space Industries (VSI) environment and provided Windows and Apache logs. The three images in this repo were extracted from slides 13, 17, and 25 of that presentation. They preserve the Splunk pixels without reconstruction. I reviewed each for credentials, personal data, and live targets before publication; none were visible in these selected captures. The original presentation remains separate and unchanged.

| Published file | Source slide | Scope of proof |
|---|---:|---|
| [Windows severity report](../evidence/windows-severity-report.png) | 13 | Saved report and counts for the displayed lab dataset. |
| [Windows monitoring dashboard](../evidence/windows-monitoring-dashboard.png) | 17 | A multi-panel monitoring view of the displayed Windows data. |
| [Apache monitoring dashboard](../evidence/apache-monitoring-dashboard.png) | 25 | A multi-panel monitoring view of the displayed Apache data. |

`WORKSPACE_INVENTORY.md` and `BOOTCAMP_RECONSTRUCTION_MAP.md`, preserved outside this repository, independently group recovered Splunk screenshots into Windows and Apache activities. They caution against treating every Splunk screenshot as a single project. The team presentation is the direct source for the selected images and establishes the project relationship.

The deck does not document which teammate performed each Splunk action. Its Windows failure alert has a threshold of 25 in the table and 28 in the explanation, so I do not quote a definitive threshold. The course activity guide says alert triggering during attack-log review was theoretical. These captures show baseline reports and dashboards; they do not verify alert firing, incident response, live monitoring, or remediation.
