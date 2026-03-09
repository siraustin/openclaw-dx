# openclaw-dx

Diagnose and fix OpenClaw gateway issues. Covers crash-loops, auth failures, config corruption, port conflicts, memory bloat, multi-profile token mismatches, and more.

## Install

### Via ClawHub
```bash
clawhub install openclaw-dx
```

### Manual
Copy `SKILL.md` to your OpenClaw skills directory:
```bash
mkdir -p ~/.openclaw/skills/openclaw-dx
cp SKILL.md ~/.openclaw/skills/openclaw-dx/
```

## What It Covers

- **Triage protocol** — parallel diagnostic commands to assess gateway state
- **15 failure modes** with symptoms, diagnosis, and fixes:
  - Failover cascade (all providers down)
  - Expired channel tokens
  - Config wiped by upgrade
  - Stale lock files
  - Device token mismatch
  - Password mismatch (multi-profile)
  - Memory bloat
  - Invalid plugin entries
  - Port conflicts / orphan processes
  - Missing configSchema in custom plugins
  - Invalid JSON from hand-edits
  - Missing gateway.remote.token
  - Config patch restart cascade
  - OPENCLAW_GATEWAY_TOKEN env var override
  - LaunchAgent plist profile mismatch
- **Memory thresholds** and Node heap tuning
- **Auth reference** — token locations, doctor --fix behavior, OAuth refresh
- **Post-fix protocol** and incident report template
- **Post-upgrade checklist**

## License

MIT
