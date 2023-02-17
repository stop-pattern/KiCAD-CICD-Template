[![kibot](https://github.com/stop-pattern/KiCAD-CICD-Template/actions/workflows/kibot.yml/badge.svg)](https://github.com/stop-pattern/KiBot-CICD-Template/actions/workflows/kibot.yml)

---

# KiBot CI/CD template repository

This repository provides different CI/CD workflows used for projects using [KiCAD](https://www.kicad.org/).

## workflows

### KiBot

[KiBot](https://github.com/INTI-CMNB/KiBot/) is used to generate all kind of documentation from a KiCAD6 project.

Whenever a file matching `*.kicad_*` changes this workflow will trigger.

The following documents are generated on every build:

```
- pcb/cad/
   - dxf/
      - AutoCAD - DXF
   - boardview - BRD
   - 3D render - STEP
- pcb/docs/
   - bom/
      - Interactive BOM - HTML
      - Octopart list - CSV
      - KiCost - XLSX (disabled)
   - schematic - PDF
- pcb/img/
   - pcb/$fab/$style/
      - PCB top - SVG
      - PCB bottom - SVG
   - render/ (disabled)
      - PCB render - PNG
   - schematic - SVG
- pcb/gerbers - ZIP
- manufactures - ZIP
   - Elecrow
   - FusionPCB
   - JLCPCB(include stencil)
   - MacroFab XYRS(bom)
   - P-Ban
   - PCBWay
```

## getting started

- [ ] hit the "use this template" button and give your project a name
- [ ] clone this new repository localy
- [ ] replace content of README.md
- [ ] PCB
   - [ ] change the filenames in `*.kicad_*` matching your repository name
   - [ ] create your PCB
- [ ] commit and push all those changes regulary to your project
