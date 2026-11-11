# Lambda Functions

Verify exact names/settings in your AWS Console before finalizing.

## visitor-http-ingest
Processes entry/exit requests through an HTTPS Lambda Function URL. Entry increments the count. Exit decrements only when the count is at least one. Input fields: `deviceId`, `action`.

## visitor-hourly-activity
Groups today's entry events by hour using Asia/Kolkata time.

## Dashboard read function
Provides current visitor count/dashboard data.

Add genuine configuration and successful test screenshots. Never publish credentials, secrets, private environment variables or sensitive account information. Review public Function URL access before sharing.
