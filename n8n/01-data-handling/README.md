# n8n - Data Handling (Set, Edit Fields, Merge, JSON)

## What this workflow covers
- Webhook (GET) input using query params
- Set / Edit Fields (map, rename, remove)
- Nested JSON structure (`user`, `meta`, `flags`)
- Merge data into a single output item
- Respond to Webhook (final JSON response)

## Test URL (local)
http://localhost:5678/webhook-test/data-handling?name=Ali&phone=03001234567&city=Peshawar

## Expected Output (example)
```json
{
  "user": { "fullName": "Ali", "mobile": "03001234567" },
  "meta": { "app": "n8n", "version": "1.0" },
  "flags": { "isVerified": false }
}
