Here's how the three-layer architecture eliminates fragmented communication:

**Detection layer** — every input channel feeds one unified event bus. IoT smoke/heat sensors, guest in-app SOS with GPS pinpointing, staff panic wearables, and CCTV anomaly detection all produce a standardized alert object with zone ID, severity signal, and timestamp. No signal is siloed at source.

**Triage & escalation engine** — an AI classifier fuses corroborating signals (a smoke sensor + a guest SOS in the same zone = high-confidence fire) to assign a severity tier in under two seconds. This gates the response protocol automatically: a Tier 1 event pages staff only; Tier 3 auto-dials emergency services and pushes a pre-built handoff packet (floor plan, hydrant map, last sensor reading, current guest count by zone) so first responders arrive informed, not blind.

**Unified comms bridge** — the three parties that normally operate in disconnected silos (distressed guest, on-site staff, emergency dispatch) are pulled into a synchronized channel. The guest gets real-time status pushes and evacuation routing. Staff see a live command picture with zone overlays and deployment assignments. Responders receive a structured data packet the moment they're notified, not after a phone handoff.

**Key design choices that prevent failure under pressure:** the system is trigger-pull by default (auto-escalation without waiting for manual confirmation), multi-redundant in detection (any one channel can start the chain), and offline-capable at the property level (local edge processing means a lost internet connection doesn't disable alerting).


