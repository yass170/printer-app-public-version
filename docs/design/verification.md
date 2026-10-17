# Verification Strategy

## Critical behaviors

- Template changes preserve the intended positions and rotations.
- Invalid batch values produce understandable diagnostics.
- An invalid or failed preview cannot be mistaken for a ready print job.
- Representative physical labels are checked separately from software rendering.

## Test layers

| Layer | Focus |
|---|---|
| Unit | Domain rules, validation and state changes without live external dependencies. |
| Integration | Consistency across application services and their storage or external-service adapters. |
| User journey | A complete path from a user action to its visible outcome, including failure states. |

## Environment checks

Barcode previews and software tests do not replace checks on the actual printer, media and production workstation.
