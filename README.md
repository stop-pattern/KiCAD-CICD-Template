[![kibot](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/kibot.yaml/badge.svg)](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/kibot.yaml)
[![oshwa](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/oshwa.yaml/badge.svg)](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/oshwa.yaml)
[![reuse](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/reuse.yaml/badge.svg)](https://github.com/nerdyscout/KiBot-CICD-Template/actions/workflows/reuse.yaml)

---

# KiBot-CICD-Template

This repository provides different CI/CD workflows with GitHub actions.

## workflows

### KiBot

[KiBot](https://github.com/INTI-CMNB/KiBot/) is used to generate all kind of documentation from a KiCAD6 project.

Whenever a file matching `pcb/*.kicad_*` changes this workflow will trigger.

The following documents are generated on every build:

```
- cad/ (disabled)
   - dxf/
      - AutoCAD - DXF
   - boardview - BRD
   - 3D render - STEP
- docs/
   - bom/
      - Interactive BOM - HTML
      - Octopart list - CSV
      - KiCost - XLSX (disabled)
   - schematic - PDF
- img/
   - pcb/
      - PCB front - SVG
      - PCB back - SVG
   - render
      - PCB render - PNG
   - schematic - SVG
- gerbers - ZIP
```

### OSHWA

On every release draft the PCB will be registered on [OSHWA](https://certification.oshwa.org/)

### REUSE

used to insure every every file got a propper license. 

## getting started

- [ ] hit the 'use this template button' and give your project a name
- [ ] clone this new repository localy.
- [ ] change the filenames in `pcb/` matching your repository name.
- [ ] replace the README.md
- [ ] [ ] make sure the licenses of `pcb/*` fit your needs.
- [ ] commit all those changes
- [ ] have fun with your PCB!
