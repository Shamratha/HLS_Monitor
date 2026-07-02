# HLS Monitor

> **Team project — Amagi Media Labs, Learning Hub 2025.** Built with [@Suraj-B12](https://github.com/Suraj-B12).
> **My contributions (frontend):**
> - Architected the React + Tailwind CSS dashboard, using Socket.io to stream real-time video/audio bitrates into live VU meters and scrollable historical charts (Recharts)
> - Built a custom `AudioSynth` engine on the Web Audio API to trigger localized siren/beep alerts for critical stream failures
> - Implemented paginated lazy-loading for error logs to keep frame rates smooth under heavy data bursts
> - Designed the frontend state layer that maps real-time backend worker updates — manifest health scores, staleness metrics, sequence drifts — into the telemetry components

A real-time HLS stream monitoring solution with live analytics, signal visualization, and health tracking.
# HLS Monitor

A real-time HLS stream monitoring solution with live analytics, signal visualization, and health tracking.

**Live Demo:** https://hls-monitor.onrender.com/

## Features

- Real-time HLS stream monitoring with 7-second polling intervals
- Live signal strength visualization with VU meters
- Auto-updating thumbnails from stream frames
- Health scoring system (0-100) based on errors and stability
- Downloadable daily log files with date selection
- Detailed video, audio, and container analysis via FFprobe
- Client-side HLS playback without server load
- Audit logging for all user operations
- Sliding window metrics for accurate health calculation
- Custom dark theme with modern UI

## Tech Stack

- Backend: Node.js, Express, MongoDB, Socket.io
- Frontend: React, Vite, Tailwind CSS, Recharts
- Analysis: FFmpeg/FFprobe

## Screenshots

The dashboard displays all monitored streams with live thumbnails and health scores. Click any stream to view detailed analytics including:

- Live signal strength meters
- Historical bitrate and signal graphs
- Video/Audio codec information
- Error logs with date filtering

## License

MIT
