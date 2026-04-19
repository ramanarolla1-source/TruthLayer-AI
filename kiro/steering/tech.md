# Tech Steering: TruthLayer AI Stack

## 1. Programming Environment
- **Primary Language:** Python 3.10+
- **Architectural Style:** Local-First, Async-first (for ElevenLabs WebSockets).
- **Core Library:** `ecdsa` for NIST P-256 cryptographic signatures.

## 2. Integration Standards
- **Voice API:** ElevenLabs (Expressive v2.5). Focus on prosody metadata (timing/pitch) over just text.
- **Trust Layer:** AetherBridge Protocol. All intent-data must be signed locally before being considered "truth."
- **Execution:** Kiro AI-First IDE Spec-Driven Development.

## 3. Coding Guidelines
- **Failure Resilience:** Code must include "offline-mode" logic. Refer to `blackout_sim.py` for intent-caching standards.
- **Security:** Never store raw audio in the cloud. Process metadata locally and sign with the Secure Enclave.
- **Gas Efficiency:** Target WASM-compatible logic for eventual deployment to Arbitrum Stylus (90% reduction target).

## 4. Key Definitions
- **The Hesitation Trap:** A specific function that calculates the delta between [Average Response Time] and [Current Token Gap].
- **Sovereign Briefing:** A summary generated via ElevenLabs that is cryptographically tied to the session ID.
