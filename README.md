# Altium Designer Libraries

A set of ready-to-use Altium Designer component libraries that I keep in one
place for prototyping boards: passives, connectors, Arduino and ESP modules,
sensors, regulators and motor drivers, most of them with 3D models.

**None of these libraries were created by me.** This repository only
collects them so they can be installed together. Credit belongs to the
original authors listed below, and each library keeps its own license.

## Contents

| Library | Format | Author / source | License |
|---------|--------|-----------------|---------|
| [`libraries/altium-lib`](libraries/altium-lib) | Source (`.SchLib`, `.PcbLib`, `.LibPkg`) + compiled `.IntLib` + 3D STEP models | Lucas Hudson, [lucashudson-eng/altium-lib](https://github.com/lucashudson-eng/altium-lib) | [GPL-3.0](libraries/altium-lib/LICENSE) |
| `libraries/Altium.IntLib` | Integrated library | Not recorded | Unknown |
| `libraries/AltiumLib1.IntLib` | Integrated library | Not recorded | Unknown |
| `libraries/AMINLIB.IntLib` | Integrated library | Not recorded | Unknown |
| `libraries/Sajad_Altium_Library.IntLib` | Integrated library | Not recorded | Unknown |

`altium-lib` is a snapshot from October 2024. Check the upstream repository
for newer parts. Its own [README](libraries/altium-lib/README.md) lists every
component by category.

If you are the author of one of the unattributed libraries, open an issue and
I will add proper credit or remove the file.

## Installation

Integrated libraries (`.IntLib`):

1. Open the **Components** panel and choose **File-based Libraries Preferences**
   from the panel menu.
2. On the **Installed** tab click **Install** and select the `.IntLib` file.

Source libraries in `altium-lib`: open the `.LibPkg` of a category and
compile it (*Project → Compile Integrated Library*), or use the prebuilt files
in [`libraries/altium-lib/libraries`](libraries/altium-lib/libraries).

## Cloning

The repository is about 700 MB, mostly 3D models. A shallow clone saves
time and space:

```sh
git clone --depth 1 https://github.com/behshadnorouzi/altium-designer-libraries.git
```
