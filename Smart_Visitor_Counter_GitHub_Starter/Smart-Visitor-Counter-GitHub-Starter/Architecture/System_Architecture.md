# System Architecture

Wokwi ESP32 simulation (Entry/Exit buttons) → HTTPS Lambda Function URL → event-ingest Lambda → DynamoDB (`VisitorCounter`, `VisitorEvents`) → dashboard read endpoint → browser dashboard.

A separate hourly-activity Lambda groups today's entry events by hour in Asia/Kolkata.

## Components
- Input: ESP32 simulated in Wokwi. Entry GPIO 22; Exit GPIO 18.
- Ingestion: `visitor-http-ingest` accepts POST fields `deviceId` and `action` (`entry` or `exit`).
- Current state: `VisitorCounter`, partition key `deviceId` (String).
- Event history: `VisitorEvents`, partition key `deviceId` (String), sort key `eventId` (String).
- Hourly activity: `visitor-hourly-activity`.
- Dashboard: separate read endpoint.

Add an architecture diagram image here. Clearly label services and arrows. The input was simulated; do not claim physical hardware deployment.
