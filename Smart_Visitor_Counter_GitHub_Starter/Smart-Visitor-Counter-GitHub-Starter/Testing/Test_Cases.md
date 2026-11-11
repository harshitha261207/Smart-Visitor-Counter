# Test Cases and Results

| ID | Test | Expected result | Captured result | Status |
|---|---|---|---|---|
| TC01 | Wi-Fi in Wokwi | Simulation connects | Confirm with screenshot | Pass as tested |
| TC02 | Entry | Count increments | HTTP 200; count incremented | Pass |
| TC03 | Exit | Count decrements | HTTP 200; count decremented | Pass |
| TC04 | Exit at zero | Count stays zero; exit rejected | `No visitors available to exit`; count 0 | Pass |
| TC05 | DynamoDB storage | Event is recorded | 20 VisitorEvents records in captured evidence | Pass |
| TC06 | Dashboard | Values refresh | Captured count 35→36; today's entries 5→6 | Pass |

The numeric values are historical screenshot evidence, not live counts. Attach the matching screenshots.
