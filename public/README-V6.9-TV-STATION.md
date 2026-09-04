# Essence Network V6.9 — TV Station Build

This release treats Essence Network as a television broadcast operation first. Internet playback is a secondary simulcast/companion service.

## Station workflow

Production sources → Preview/Program → Graphics/Audio → Master Control → Scheduled Playout → Transmission Output → external broadcast I/O/encoder/transmitter.

## Studio
- Master Control with TAKE, BACKUP, EMERGENCY, SCHEDULED and STOP SERVICE actions
- Preview / Program monitors
- Camera + microphone, screen share and local media
- Scenes and broadcast graphics
- Browser audio gain/metering
- Master recording
- Transmission output map (SDI, NDI, IP/Encoder, ASI, File/Archive)

## Control Centre
- Create and edit television services
- Channel number and call sign
- Video/audio format
- Transmission output definition
- Optional web simulcast URL
- Programme/EPG management

## Important deployment boundary
The software is the production/master-control layer. A physical SDI/NDI/IP/ASI interface, encoder, playout server and the broadcaster's licensed distribution/transmitter chain are required for real-world TV transmission. The web HLS player is not the television transmitter.
