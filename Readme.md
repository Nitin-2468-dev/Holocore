# HoloCore

Experimental light-field display software and hardware.

HoloCore generates multi-view quilts from a 3D scene and sends them
through a light-field shader to a lenticular display.

![Controller](Images/controller.png)

## What I've built

| Part | Status |
|---|---|
| Custom 3D editor | Done |
| 48-view rendering | Done |
| 6 × 8 quilt generation | Done |
| Light-field shader | Done |
| Separate display output process | Done |
| Shared-memory frame transfer | Done |
| Multi-monitor output | Done |
| Custom UI system | Done |

![Quilt](Images/quilt.png)

## Pipeline

| Stage | Description |
|---|---|
| 1 | 3D Scene |
| 2 | 48 Views |
| 3 | Quilt |
| 4 | Light-field Shader |
| 5 | Display |

![Output](Images/Interlaced_output.png)

> You know what this reminds me of?
>
> ![](https://i.pinimg.com/736x/9a/6c/9a/9a6c9a434d84276756b890d7923f8865.jpg)
>
> **Reverse Flash.**

## Hardware

The goal is to build a physical light-field display using an LCD,
lenticular sheet, and acrylic optical stack.

I want to build this.

![Concept](https://cdn.hackclub.com/019e2cc1-1fb9-767f-bb08-b036db4d9f16/Screenshot%202026-05-15%20181331.png)

And after some calculation:

![Calculations](https://cdn.hackclub.com/019e2cc1-7022-76f6-b8ab-749e2f066d06/Screenshot%202026-05-15%20182731.png)

I started on the CAD:

![CAD](https://cdn.hackclub.com/019e2cc2-2b59-72cc-909d-3f6e8645f5b7/Screenshot%202026-05-15%20214922.png)

![CAD](https://cdn.hackclub.com/019e2cc2-5077-771a-818b-69048b805a7f/Screenshot%202026-05-15%20224108.png)

And my "ahh moment":

[Looking Glass — Light Field Display](https://www.youtube.com/watch?v=ImMIfI01zs8)


| Step 1 | Step 2 | Step 3 | Step 4 |
|---|---|---|---|
| ![Step 1](https://cdn.hackclub.com/019e2cc3-d4b5-7a91-b71d-24a6942bae6f/Screenshot%202026-05-15%20225328.png) | ![Step 2](https://cdn.hackclub.com/019e2cc3-e8c3-77d6-98a8-70c3aad835f1/Screenshot%202026-05-15%20225250.png) | ![Step 3](https://cdn.hackclub.com/019e2cc3-fb08-7ab4-8e7e-962bb88a93a4/Screenshot%202026-05-15%20225400.png) | ![Step 4](https://cdn.hackclub.com/019e2cc4-09f5-7ecc-bb3b-e02a371ef933/Screenshot%202026-05-15%20231229.png) |

The glass block is used to **add depth** between the display and the
lenticular sheet.

![CAD](Images/cad.png)

The CAD files are available on Onshape and in the repository.

## Software

The current software implementation is developed in
[HoloCore-farmware](https://github.com/Nitin-2468-dev/HoloCore-farmware).

## Project

HoloCore-farmware is the software/firmware implementation of
[HoloCore](https://github.com/Nitin-2468-dev/HoloCore).

## Run

```bash
uv sync
uv run Core.py
```

----

### License See [LICENSE](LICENSE). 
