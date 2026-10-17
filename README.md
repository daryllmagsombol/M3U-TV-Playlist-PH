# M3U-TV-Playlist-PH

Philippine-focused IPTV playlist for M3U-compatible players.

## Import

Point your player at this URL:

```
https://raw.githubusercontent.com/daryllmagsombol/M3U-TV-Playlist-PH/main/index.m3u
```

## What's in it

A one-time sync (2026-10-17) of the **non-DRM** streams from
[ryansnetcafe/ott-playlist](https://github.com/ryansnetcafe/ott-playlist)
(`ryansnetcafe.m3u`). Only entries with no ClearKey/DRM configuration were kept;
every DRM-configured entry was omitted.

- 117 entries total
- 103 DASH (`.mpd`) streams
- 1 HLS (`.m3u8`) stream
- 13 internet-radio audio streams

## Migration note

The old **PH-US.m3u** list has been **replaced, not merged**. Both its filename
and raw URL changed — the playlist is now `index.m3u`. Update any old link that
pointed at `PH-US.m3u` to the import URL above.

## Playback caveats

- **DASH streams need a DASH-capable player.** Not every M3U player handles
  `.mpd`/DASH; "non-DRM" does not mean "works everywhere".
- Stream tokens embedded in the URLs **may expire**, which can break playback
  over time.
- Playback also depends on your network, the request headers/User-Agent your
  player sends, codec support, and the app itself.
- This repository makes **no promise** that any stream plays or stays online.

## Source & attribution

Streams come from
[ryansnetcafe/ott-playlist](https://github.com/ryansnetcafe/ott-playlist).
All rights belong to their respective owners. No DRM was bypassed or decrypted;
DRM-configured entries were simply omitted.
