# Essence Network V6.3 — Friendly Production Studio

This build adds a browser-first production control surface designed to be easy for operators to learn.

## Working browser features
- Camera + microphone capture with Web Audio microphone gain and live meter
- Screen sharing
- Local video package loading
- Preview / Program monitors
- TAKE and Space-bar switching
- Camera + Screen picture-in-picture scene
- Lower-third / Breaking / LIVE graphics
- Connected network graphic TAKE/OFF AIR through the Essence API
- Composed Program canvas so graphics are included in local recordings
- Local WebM program recording with microphone audio when available
- Rundown/cue workflow
- Responsive UI and local demo mode

## Broadcast-engine boundary
The browser studio is the operator interface and local compositor. It is not a replacement for a dedicated transmission encoder. For true RTMP/SRT/HLS transmission, the next layer should be a server-side media engine (for example FFmpeg/MediaMTX) connected to the Program output. FFmpeg is designed for recording, transcoding and streaming media workflows.

## Deployment
The existing Express API serves `/studio` and `/studio-assets`. Run the project with Node 22+ after installing dependencies. The Local Demo button can be used without API login to rehearse the studio UI in a browser.
