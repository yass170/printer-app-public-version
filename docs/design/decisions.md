# Design Decisions

## 1. Separate authoring from production printing

**Benefit.** Operators can use prepared templates without editing their design.

**Trade-off.** The two applications must agree on the meaning of shared layouts.

## 2. Preview and print output follow consistent geometry

**Benefit.** The preview can expose layout and data problems before a print job.

**Trade-off.** Printer behavior still requires physical validation on the target device.

## 3. Keep printer access behind adapters

**Benefit.** Domain and UI behavior can be tested without issuing a physical print.

**Trade-off.** Software tests cannot establish the quality of a real printed label.
