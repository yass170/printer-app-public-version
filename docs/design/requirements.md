# Product Requirements

A Windows desktop toolset for designing reusable label layouts and printing batches of labels on Zebra-compatible printers.

## Users

| Role | Expected outcome |
|---|---|
| Template administrator | Create, edit and verify label layouts and manage shared template locations. |
| Production operator | Select a template, load a batch, preview labels and confirm the printer destination. |

## Functional scope

| Capability | User outcome |
|---|---|
| Visual template editor | Compose text, images, shapes and barcodes in a WYSIWYG label workspace. |
| Layout manipulation | Select, move, resize, rotate and undo changes to label elements. |
| Template library | Find and reuse layouts from configured shared locations. |
| Batch verification | Check how incoming values map onto a chosen label and inspect diagnostic results. |
| Operator preview | Review labels using the batch’s actual values before printing. |
| Printer integration | Select a Windows printer and submit confirmed label output. |

## Main user journey

1. An administrator prepares and verifies a reusable label template.
2. An operator chooses that template and opens a batch file.
3. The application validates the input and renders a preview.
4. The operator checks the result and confirms printing.

## Acceptance priorities

- Template changes preserve the intended positions and rotations.
- Invalid batch values produce understandable diagnostics.
- An invalid or failed preview cannot be mistaken for a ready print job.
- Representative physical labels are checked separately from software rendering.

## Product constraint

Barcode previews and software tests do not replace checks on the actual printer, media and production workstation.
