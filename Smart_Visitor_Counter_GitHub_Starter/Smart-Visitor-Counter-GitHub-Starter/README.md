# Smart Visitor Counter

Cloud-based visitor monitoring prototype that records entry/exit events, maintains a current count, stores event history and displays activity in a browser dashboard.

## Project status
- AWS backend: deployed and tested in the project environment.
- Input: ESP32 workflow simulated using Wokwi.
- Dashboard: executed in a browser.
- Physical hardware deployment: not completed.

## Services and tools
Wokwi ESP32 simulation, HTML/CSS/JavaScript, AWS Lambda, Lambda Function URLs, Amazon DynamoDB and Amazon CloudWatch.

## Workflow
1. Wokwi generates an entry or exit event.
2. The ESP32 simulation sends an HTTPS request to a Lambda Function URL.
3. Lambda updates the visitor count and records the event in DynamoDB.
4. Dashboard endpoints provide current count and hourly entry activity.

## Repository contents
- Architecture: system workflow and architecture.
- AWS_Configuration: Lambda, DynamoDB and CloudWatch notes.
- Wokwi_Simulation: simulation details.
- Testing: test cases and results.
- Screenshots: actual project evidence.
- Reports: final report and presentation.

## Team
| Name | Roll number |
|---|---|
| B. Arun Reddy | 2503A51155 |
| A. Harshitha | 2503A51156 |
| B. Preethi | 2503A51159 |
| P. Trishul | 2503A51164 |
| Arshiya Taranum | 2503A51175 |

SR University, Warangal | School of CS & AI | CSE | Academic Year 2026–2027

**This is a documentation/evidence repository. It does not claim to contain source code unless source files are added. Never upload AWS credentials, secret keys, passwords or session tokens.**
