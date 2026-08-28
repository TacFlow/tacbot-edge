# TacBot Edge

Edge device SDK for the TacFlow swarm ecosystem. Connect IoT devices, cameras, and sensors to your TacFlow agents.

## Features

- **Native Go agent** — runs on Raspberry Pi, Linux, macOS, Windows
- **Camera support** — capture photos, record video, motion detection
- **Sensor integration** — temperature, humidity, pressure, motion
- **Swarm communication** — NATS broker for real-time agent messaging
- **Over-the-air updates** — remote skill deployment
- **Encrypted payloads** — AES-256-GCM for sensitive edge data

## Quick Start

```bash
# Install on Raspberry Pi (64-bit)
curl -fsSL https://get.tacflow.ai/install-edge.sh | bash

# Start the edge agent
tacbot-edge start --swarm YOUR_SWARM_ID

# Test camera
tacbot-edge camera capture --output test.jpg
```

## Supported Devices

| Device | Status | Notes |
|--------|--------|-------|
| Raspberry Pi 4/5 | ✅ | 64-bit, camera module |
| Raspberry Pi Zero 2 W | ✅ | Limited RAM, no video |
| Jetson Nano | ✅ | GPU acceleration |
| Linux x86_64 | ✅ | USB cameras |
| Windows | ✅ | DirectShow cameras |
| macOS | ✅ | AVFoundation cameras |

## License

MIT — Open Source
