# free-iptv-threat-intel

Open-source threat intel on malicious domains found in free IPTV playlists, with scan verdicts and timestamps.

## Contents

- `scan_results.json` - domain risk verdict database
- `summary_report.md` - latest scan summary snapshot

## Data Schema

Each key is a domain (or host:port) and value follows:

```json
{
  "malicious": 0,
  "suspicious": 0,
  "last_scanned": "2026-03-05T06:36:41+00:00"
}
```

## Notes

- Verdicts are time-sensitive and may change over time.
- This dataset is intended for defensive/security research and risk triage.
- A domain listed here is an indicator, not standalone proof of compromise.

## Source

Data is generated from the IPTV playlist scanning pipeline in the `IPTV_playlist_manager` project.

Generated (UTC): 2026-03-05T09:43:51Z
