# Splunk monitoring: Windows and Apache lab data

In 2024, I worked with four classmates on a UC Berkeley cybersecurity bootcamp project for Virtual Space Industries (VSI), a fictional company. Our team used Splunk to review provided Windows and Apache logs, build reports and dashboards, and present an analysis of the simulated attack data.

I am named on the [team presentation described in the evidence notes](docs/evidence-notes.md). The presentation does not assign individual ownership of each Splunk search or dashboard. The examples below are team results, not claims that I configured every panel myself.

| Example | Evidence | What the capture shows |
|---|---|---|
| Windows event summary | [Severity report](evidence/windows-severity-report.png) | Splunk categorized 9,528 events: 8,870 informational and 658 high severity. The label is from the lab data; it does not by itself confirm an incident. |
| Windows monitoring | [Dashboard](evidence/windows-monitoring-dashboard.png) | Panels chart users and event signatures over time, with a deleted-account count and user counts. This is a baseline monitoring view, not proof of attack detection. |
| Apache monitoring | [Dashboard](evidence/apache-monitoring-dashboard.png) | Panels show client geography, HTTP methods over time, URI counts, a referrer total, and countries. The capture is a monitoring view, not proof that the requests were malicious. |

The team presentation also describes scheduled alerts and analysis of separate attack logs. I have not published the underlying alert configurations or attack-log searches here, so this case study does not claim that alerts fired, an incident was confirmed, or a live environment was monitored. See [evidence notes](docs/evidence-notes.md) for the source and limits.
