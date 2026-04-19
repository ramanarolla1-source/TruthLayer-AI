# Technical Design: TruthLayer Architecture

## Components
1. **Signal Catcher:** WebSocket listener for ElevenLabs audio streams.
2. **Intent Decoder:** Logic engine running the "Hesitation Trap" rules.
3. **Hardware Signer:** NIST P-256 signature generator (AetherBridge protocol).

## Data Flow
ElevenLabs (Audio) -> Kiro Agent (Prosody Analysis) -> Local Enclave (Signing) -> Briefing Output.
