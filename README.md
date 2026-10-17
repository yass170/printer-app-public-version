# Printer App — Label Design and Production Printing

A Windows desktop toolset for designing reusable label layouts and printing batches of labels on Zebra-compatible printers.

Administrators prepare reusable label templates; operators load those templates with batch data, inspect the output and confirm printing. The project separates template authoring from production use while keeping the interpretation of label geometry consistent.

## Users

| Role | Use |
|---|---|
| Template administrator | Create, edit and verify label layouts and manage shared template locations. |
| Production operator | Select a template, load a batch, preview labels and confirm the printer destination. |

## Main features

- **Visual template editor.** Compose text, images, shapes and barcodes in a WYSIWYG label workspace.
- **Layout manipulation.** Select, move, resize, rotate and undo changes to label elements.
- **Template library.** Find and reuse layouts from configured shared locations.
- **Batch verification.** Check how incoming values map onto a chosen label and inspect diagnostic results.
- **Operator preview.** Review labels using the batch’s actual values before printing.
- **Printer integration.** Select a Windows printer and submit confirmed label output.

## Typical workflow

1. An administrator prepares and verifies a reusable label template.
2. An operator chooses that template and opens a batch file.
3. The application validates the input and renders a preview.
4. The operator checks the result and confirms printing.

## Project structure

```text
printer-app-public-version/
├── administration/
│   ├── csharp/
│   │   ├── module-003/
│   │   │   └── module-001/
│   │   ├── src/
│   │   │   ├── app/
│   │   │   ├── application/
│   │   │   ├── domain/
│   │   │   └── infrastructure/
│   │   └── tests/
│   ├── docs/
│   │   ├── decisions/
│   │   │   └── README.md
│   │   ├── issue/
│   │   ├── specifications/
│   │   ├── technical/
│   │   └── user/
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   ├── scripts/
│   │   └── tests/
│   ├── tools/
│   │   └── typography/
│   └── README.md
├── docs/
│   ├── design/
│   │   ├── decisions.md
│   │   ├── requirements.md
│   │   └── verification.md
│   └── module-001/
├── operateur/
│   ├── backend/
│   │   ├── domain/
│   │   ├── resources/
│   │   │   └── typography/
│   │   ├── services/
│   │   └── tests/
│   ├── docs/
│   │   ├── decisions/
│   │   │   └── README.md
│   │   ├── issue/
│   │   ├── specifications/
│   │   ├── technical/
│   │   └── user/
│   ├── frontend/
│   │   ├── controllers/
│   │   ├── dialogs/
│   │   ├── module-007/
│   │   ├── tests/
│   │   └── app.py
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   ├── module-005/
│   │   └── module-001/
│   │       ├── module-002/
│   │       ├── src/
│   │       └── README.md
│   ├── module-006/
│   ├── packaging/
│   ├── scripts/
│   │   └── tests/
│   ├── pyproject.toml
│   └── README.md
├── ARCHITECTURE.md
└── README.md
```

[Complete directory structure](docs/design/structure.md)

| Area | Responsibility |
|---|---|
| Administration application | C#/.NET with Avalonia and MVVM for template editing and verification. |
| Operator application | Python/Tkinter interface for batch loading, preview and printing. |
| Domain and application layers | Label concepts, editing operations, verification and use cases. |
| Rendering and printing adapters | Preview generation, barcode handling and Windows printer access. |
| Shared documents | External template definitions and batch inputs exchanged by the two applications. |

## Technology

C#/.NET, Avalonia, MVVM, Python, Tkinter, XML and ZPL.

## Engineering

- [Architecture](ARCHITECTURE.md)
- [Product requirements](docs/design/requirements.md)
- [Design decisions](docs/design/decisions.md)
- [Verification strategy](docs/design/verification.md)

Barcode previews and software tests do not replace checks on the actual printer, media and production workstation.

---

Source code, operational configuration and project-specific data are withheld for confidentiality.
