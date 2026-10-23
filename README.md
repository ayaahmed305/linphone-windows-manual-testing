
# Linphone Desktop (Windows): Manual Testing Project

> An end-to-end manual testing project for the Linphone softphone on Windows, planned and executed following ISTQB principles.
> This is a personal learning and portfolio project. It is not affiliated with or endorsed by Belledonne Communications.

**Status: in progress.** Documents and results are added as the work is completed. See the checklist below.

## Overview

[Linphone](https://www.linphone.org/) is an open-source VoIP application for audio/video calls and instant messaging over the SIP protocol, developed by Belledonne Communications (France).

In this project I act as test lead and tester: I define the scope, analyze risks, design and execute test cases, log defects, and write the final report, covering the full test process from planning to closure.

| | |
|---|---|
| **Application under test** | Linphone Desktop VERSION_HERE |
| **Platform** | Windows 11 (build 26200.9711) |
| **Duration** | 2026-10-20 to 2026-10-30 |
| **Role** | Test Lead and Tester (solo project) |
| **Test type** | Manual, black-box, risk-based |

## Project Status

- [x] Repository and README
- [ ] Test plan
- [ ] Risk analysis
- [ ] Test scenarios
- [ ] Test cases
- [ ] Test execution and bug reports
- [ ] Summary report

## Scope

**In scope**
- Account management (registration, login, multiple accounts)
- Audio and video calls, call controls (hold, mute, transfer, DTMF)
- Instant messaging and file sharing
- Contacts and call history
- Settings (audio, video, network, encryption, codecs)
- Installation, upgrade, and uninstall
- Basic security checks (ZRTP/SRTP) verified with Wireshark
- Behavior under poor network conditions (packet loss, latency)
- Usability and basic accessibility

Features that do not exist in the tested version are removed from scope and noted in the test plan.

**Out of scope**
- Mobile and other desktop platforms (single device available)
- Flexisip server and Liblinphone SDK
- Load testing and penetration testing

## Approach

The project follows the ISTQB test process:

1. **Planning:** scope, objectives, entry/exit criteria
2. **Analysis:** documentation and release notes review, risk analysis
3. **Design:** test scenarios and test cases using standard techniques
4. **Implementation:** environment, accounts, tools
5. **Execution:** smoke, functional, non-functional, exploratory
6. **Reporting and closure:** defect triage, summary report, lessons learned

**Test design techniques:** equivalence partitioning, boundary value analysis, state transition testing, decision tables, error guessing, and session-based exploratory testing.

**Risk-based prioritization:** areas with the highest likelihood and impact (call setup, registration, encryption, audio quality) receive the deepest coverage.

## Tools

| Tool | Purpose |
|---|---|
| Wireshark | Inspect SIP signaling and RTP/SRTP media |
| Clumsy | Simulate packet loss, delay, and jitter |
| OBS Studio | Screen and audio recording |
| Google Sheets / Excel | Test cases, execution results, and bug log |
| GitHub | Version control and documentation |

## Repository Structure

```
docs/            Test plan, risk analysis, scenarios, summary report, AI usage policy
test-cases/      Test cases grouped by feature area
traceability/    Scenario-to-test-case matrix
bug-reports/     Defect reports
reports/         Daily reports and exploratory session notes
evidence/        Screenshots and recordings
templates/       Test case and bug report templates
```

## Use of AI

AI tools are used to explain concepts, draft test case ideas, and polish reports. Every AI-generated output is reviewed and verified manually before being included. No credentials or personal data are shared with AI tools.

## Limitations

- Testing is performed on a single version and a single device, so results may not generalize to other environments.
- Testing can show the presence of defects, not their absence.
- Network results depend on conditions at the time of testing.

## Author

**Aya Ahmed**
[LinkedIn](https://www.linkedin.com/in/aya-ahmed-9b844b23a)
