# HoloCore

Experimental light-field display software and hardware.

HoloCore generates multi-view quilts from a 3D scene and sends them
through a light-field shader to a lenticular display.

*click on it*
[![Controller](Images/Controller.png)](https://youtu.be/qHE5rNMxpnc)

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

![Quilt](Images/Quilt.png)

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

<img src="https://cdn.hackclub.com/019eeb73-149e-7e7b-a862-a1c68f8b2347/ezgif.com-coalesce.gif" alt="Project thumbnail" class="w-full h-full object-cover" data-v-ae87ac37="">

And after some calculation:

![Calculations](https://cdn.hackclub.com/019e2cc1-7022-76f6-b8ab-749e2f066d06/Screenshot%202026-05-15%20182731.png)

And "ahh moment":

[Looking Glass — Light Field Display](https://www.youtube.com/watch?v=ImMIfI01zs8)


| Step 1 | Step 2 | Step 3 | Step 4 |
|---|---|---|---|
| ![Step 1](https://cdn.hackclub.com/019e2cc3-d4b5-7a91-b71d-24a6942bae6f/Screenshot%202026-05-15%20225328.png) | ![Step 2](https://cdn.hackclub.com/019e2cc3-e8c3-77d6-98a8-70c3aad835f1/Screenshot%202026-05-15%20225250.png) | ![Step 3](https://cdn.hackclub.com/019e2cc3-fb08-7ab4-8e7e-962bb88a93a4/Screenshot%202026-05-15%20225400.png) | ![Step 4](https://cdn.hackclub.com/019e2cc4-09f5-7ecc-bb3b-e02a371ef933/Screenshot%202026-05-15%20231229.png) |

The glass block is used to **add depth** between the display and the
lenticular sheet.

![CAD](Images/cad.png)

The CAD files are available on Onshape and in the repository.

### (Bill of Materials)

| Component                                            | Purpose                                           |   Qty. |                Cost | Distributor                                                                                                   |
| ---------------------------------------------------- | ------------------------------------------------- | -----: | ------------------: | ------------------------------------------------------------------------------------------------------------- |
| Waveshare 7" 1024×600 HDMI IPS Capacitive LCD        | Main display panel                                |      1 |     ₹4,389 / $48.28 | [Robu.in](https://robu.in/product/waveshare-7inch-1024x600-hdmi-ips-low-power-capacitive-lcd-c-touch-screen/) |
| Print6D 50 LPI Lenticular Sheets (6"×4", pack of 10) | Optical lens layer for view separation            | 1 pack |       ₹990 / $10.89 | [Amazon.in](https://www.amazon.in/gp/product/B0D91RVKWT)                                                      |
| 3D-printed parts                                     | Mechanical frame, mounts, and alignment parts     |      — |            ₹0 / $0* | Printing Legion India                                                                                         |
| A4 Guillotine Paper Cutter                           | Cutting lenticular sheets and prototype materials |      1 |     ₹1,044 / $11.48 | [Amazon.in](https://www.amazon.in/Toners-Trimmer-Machine-Guillotine-Hand-held/dp/B0FBHK7YK9)                  |
| **Total**                                            |                                                   |        | **₹6,423 / $70.65** |                                                                                                               |

**Exchange rate:** approximately ₹91.0 = $1 USD, recorded on 21/08/2026.

[**CSV file**](./holocore-BOM.csv)


## Software

The current software implementation is developed in
[HoloCore-farmware](https://github.com/Nitin-2468-dev/HoloCore-farmware).

## Releases

| Platform | Download |
|---|---|
| Windows | [Latest release](https://github.com/Nitin-2468-dev/HoloCore-farmware/releases/latest) |
| Linux | Coming soon |

## Run the sorce code

```bash
uv sync
uv run Core.py
```

## If you want the strugles 
[Macondo Project](https://macondo.hackclub.com/projects/952)

----

### License See [LICENSE](LICENSE). 
