# Feature: Vocal Intent & Hesitation Detection
**Status: Spec-First**

## User Stories
1. **As a Leader**, I want to detect "False Yes" responses so I can address misaligned expectations before they cause ghosting.
2. **As a Developer**, I want vocal markers signed via NIST P-256 so the intelligence briefings are tamper-proof.

## Acceptance Criteria
- **GIVEN** a "Yes" token is detected in the transcript
- **WHEN** the associated audio has a [Response_Time] > [Baseline * 3]
- **THEN** flag as "High Hesitation" and assign a Severity Score > 80.
