# The Silent Server (Backend Debugging Assignment)

This API is intentionally broken.
Your task is to fix it and generate your access token.

## Setup

```bash
npm install
npm start
```

Server runs at: `http://localhost:3000`

## Assignment

This is a simple API that generates a unique access token for your job application.
Currently, the `/token` endpoint times out or errors.
Fix it, generate your token, and submit it.

After fixing, run:

```bash
curl -X POST http://localhost:3000/token \
  -H "Content-Type: application/json" \
  -d '{"email":"candidate@gmail.com"}'
```

Expected shape:

```json
{
  "status": "success",
  "token": "BE-DEV-7721-<base64-hash>"
}
```
