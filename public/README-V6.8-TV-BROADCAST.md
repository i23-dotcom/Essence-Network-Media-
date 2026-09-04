# Essence Network V6.8 — TV Broadcast Studio

V6.8 corrects the architecture: Essence Network is being built as a **television broadcast operation**, not an IPTV-only application.

## Primary broadcast chain

Studio sources → Preview/Program → Master Control → Graphics/Audio → Playout/Transmission → TV distribution.

The web player and HLS/RTMP outputs are treated as **secondary simulcast / distribution paths**, not the definition of the TV station.

## Production features
- Master Control with service status and TAKE TO AIR.
- Camera, microphone, screen and media sources.
- Program/Preview switching.
- Broadcast graphics.
- Audio controls and metering.
- Rundown and programme scheduling.
- Master recording.
- TV service/channel management with channel number, call sign, video/audio format and transmission output.
- Optional web simulcast.

## Real transmission boundary
A browser cannot directly drive SDI/ASI hardware or a terrestrial/satellite transmitter. For physical TV transmission, deploy the Studio control plane alongside an authorised local broadcast I/O and encoder/transmitter chain (for example SDI/NDI/IP contribution into a playout/encoder system). The software now models that boundary explicitly instead of presenting HLS playback as the core TV service.
