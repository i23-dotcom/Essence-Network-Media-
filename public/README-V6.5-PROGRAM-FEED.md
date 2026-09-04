# Essence Network V6.5 — Program Live Feed

V6.5 connects the browser Program canvas to the server FFmpeg media engine.

## Flow
1. Operator opens Production and selects a camera/screen/media scene.
2. TAKE switches Preview to Program.
3. Graphics are composited into the Program canvas.
4. Broadcast → START PROGRAM FEED captures that canvas with the browser audio track.
5. Media chunks are sent to `/api/workspace/program-stream/chunk`.
6. FFmpeg receives WebM on stdin and publishes HLS at `/live/program.m3u8` or RTMP to the configured destination.

## Important
This is a browser-to-server contribution path, not a replacement for a dedicated hardware/encoder stack. A production deployment should use HTTPS, sufficient server CPU, persistent storage for HLS, and a proper media edge/CDN.
