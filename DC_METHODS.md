# Device Connection Methods — 2026-10-21

> Reference for restoring laptop↔cloud connectivity. Vague mode — no strategy details.

## Method 1: DC Remote (easiest, recommended)

One command in any terminal on the laptop, keep it open:

```
npx @wonderwhy-er/desktop-commander@latest remote
```

- No install needed — npx pulls it automatically
- Keep the window open; closing it kills the connection
- Device ID (LenovoLaptop): `24123e3e-6795-430b-abf6-32e186477523`
- Connector UUID on claude.ai: `daef668b`

## Method 2: RC Session (Remote Control)

Start from any claude.ai thread:
- Use `start_remote_control` with `environment_id: env_01NgJTR6zYm3KYGtfCvGCPGF`
- Or click "Remote Control" in the Claude desktop app

## Method 3: DC Clone (auto-restart)

Scheduled task — starts automatically at login and every 15 min:

```powershell
Start-ScheduledTask DcCloneServer
Get-ScheduledTask Cloud_DC_Watchdog   # check watchdog status
```

## Repair sequence (if connection lost)

```powershell
# Step 1: Kill stale node processes
Get-Process node -ErrorAction SilentlyContinue | Stop-Process -Force

# Step 2: Restart DC Clone
Start-ScheduledTask DcCloneServer

# Step 3: Restart DC Remote (in a new window, keep open)
npx @wonderwhy-er/desktop-commander@latest remote
```

## Watchdog

`Cloud_DC_Watchdog` scheduled task auto-restarts DC Clone + DC Remote at login and every 15 min. If it's missing, re-register it.

---
*Private/infrastructure only — no strategy details here.*
