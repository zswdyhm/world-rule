# IPTV

Curated English IPTV channels, stress tested for stable playback.

## Channels

| File | Channels | Categories | Description |
|------|----------|------------|-------------|
| `english-curated.m3u` | 126 | 22 | Stable playback verified (ffmpeg decode speed ≥2x) |

## Usage

Add to any IPTV player (APTV, VLC, IINA, etc.):

```
https://raw.githubusercontent.com/zswdyhm/world-rule/main/iptv/english-curated.m3u
```

EPG (Electronic Program Guide):

```
https://epgshare01.online/epgshare01/epg_ripper_ALL_SOURCES1.xml.gz
```

## Categories

| Category | Count | Avg Speed |
|----------|-------|-----------|
| News | 21 | 9.9x |
| Documentary | 14 | 6.2x |
| Sports | 13 | 5.7x |
| Business | 11 | 9.2x |
| Movies | 10 | 9.3x |
| Music | 8 | 9.7x |
| Lifestyle | 7 | 4.4x |
| Entertainment | 6 | 4.4x |
| Education | 5 | 12.5x |
| Kids | 4 | 8.2x |
| Series | 4 | 10.1x |
| Cooking | 3 | 6.0x |
| Culture | 3 | 10.8x |
| Family | 3 | 6.1x |
| Outdoor | 3 | 4.3x |
| Travel | 3 | 6.2x |
| Animation | 2 | 10.6x |
| Comedy | 2 | 11.7x |
| BBC | 1 | 8.0x |
| Relax | 1 | 3.6x |
| Science | 1 | 5.5x |
| Weather | 1 | 15.6x |

## Quality Assurance

Every channel passed a two-stage test:
1. **Connectivity test**: HTTP 200 + response latency ≤5s (curl)
2. **Stress test**: ffmpeg actual decode for 15 seconds, playback speed ≥2x

Channels that passed connectivity but failed stable playback (e.g. Pluto TV, Vevo) were removed.

## Source

Channels sourced from [iptv-org/iptv](https://github.com/iptv-org/iptv).
