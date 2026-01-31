# HackPad

A custom 6-key mechanical macro pad with RGB lighting, OLED display, and rotary encoder, designed for productivity and customization.

![HackPad Assembled](JONAHS%20HACKPAD/JONAHS%20HACKPAD/FUSION%20Photos/Assembled.png)

## Overview

HackPad is a compact, open-source macro pad featuring 6 hot-swappable mechanical key switches with individual RGB backlighting. Perfect for streamers, content creators, developers, and power users who want quick access to custom shortcuts and macros.

## Features

- **6 Hot-Swappable Mechanical Switches** - Compatible with Cherry MX-style switches
- **Per-Key RGB Lighting** - Individually addressable SK6812MINI LEDs for stunning lighting effects
- **OLED Display** - Real-time feedback and status information
- **Rotary Encoder** - Volume control, scrolling, or custom functions
- **ESP32 Microcontroller** - WiFi and Bluetooth connectivity
- **Custom 3D-Printed Case** - Sleek and professional design
- **Open-Source** - Full hardware and design files available

## Hardware Specifications

### Components

- **Microcontroller**: ESP32 (with WiFi & Bluetooth)
- **Switches**: 6x hot-swappable mechanical key switches (Cherry MX compatible)
- **RGB LEDs**: 11x SK6812MINI addressable RGB LEDs
- **Display**: OLED display module
- **Encoder**: Rotary encoder with push button
- **PCB**: Custom 2-layer PCB design

### PCB Details

![PCB Design](JONAHS%20HACKPAD/JONAHS%20HACKPAD/KICAD%20Photos/PCB%20Image%20.png)

- **Size**: Compact form factor optimized for 6 keys
- **Layers**: 2-layer PCB
- **Design Tool**: KiCAD 9.0.7

### Schematic

![Schematic](JONAHS%20HACKPAD/JONAHS%20HACKPAD/KICAD%20Photos/Schematic%20Image%20.png)

## Repository Contents

```
HackPad/
├── JONAHS HACKPAD/
│   ├── BOM/
│   │   └── ibom.html                  # Interactive Bill of Materials
│   ├── FUSION Photos/
│   │   ├── Assembled.png              # 3D render of assembled device
│   │   ├── Case.png                   # Case design
│   │   └── Lid.png                    # Lid design
│   ├── KICAD Files/
│   │   └── [Gerber files]             # PCB manufacturing files
│   ├── KICAD Photos/
│   │   ├── 3d PCG Image.png           # 3D PCB view
│   │   ├── PCB Image .png             # PCB layout
│   │   └── Schematic Image .png       # Circuit schematic
│   ├── PCB Pro Files/
│   │   └── PRO/
│   │       ├── PRO.kicad_pcb          # KiCAD PCB design file
│   │       ├── PRO.kicad_sch          # KiCAD schematic file
│   │       ├── PRO.kicad_pro          # KiCAD project file
│   │       ├── PRO.step               # 3D model (STEP format)
│   │       ├── PRO.stl                # 3D model (STL format)
│   │       ├── JLCPCB/                # Production files for JLCPCB
│   │       └── bom/                   # Bill of Materials
│   └── STEPS/
│       ├── Assembled case.step        # Full assembly STEP file
│       ├── JONAH BASE.step            # Case base STEP file
│       └── JONAHS LID.step            # Case lid STEP file
```

## Bill of Materials (BOM)

For a complete, interactive bill of materials with component placement, open the `BOM/ibom.html` file in your web browser.

### Key Components

- 6x Mechanical Key Switches (Cherry MX compatible)
- 6x Hot-swap sockets
- 11x SK6812MINI RGB LEDs
- 1x ESP32 Development Board
- 1x OLED Display Module
- 1x Rotary Encoder
- Various resistors, capacitors, and connectors (see BOM for details)

## PCB Manufacturing

### Ordering PCBs

The Gerber files for PCB manufacturing are located in:
- `JONAHS HACKPAD/JONAHS HACKPAD/KICAD Files/` - Standard Gerber files
- `JONAHS HACKPAD/JONAHS HACKPAD/PCB Pro Files/PRO/JLCPCB/` - JLCPCB-optimized files

#### Recommended Settings for JLCPCB

- **Base Material**: FR-4
- **Layers**: 2
- **Thickness**: 1.6mm
- **Surface Finish**: HASL or ENIG
- **Copper Weight**: 1 oz
- **Remove Order Number**: Yes (optional)

Simply upload the Gerber files to your preferred PCB manufacturer (JLCPCB, PCBWay, OSH Park, etc.).

## 3D Printed Case

### Files

The case is designed in Fusion 360 and exported as STEP files:

- `STEPS/Assembled case.step` - Complete assembly for preview
- `STEPS/JONAH BASE.step` - Bottom case part
- `STEPS/JONAHS LID.step` - Top lid part

### Printing Recommendations

- **Material**: PLA or PETG
- **Layer Height**: 0.2mm
- **Infill**: 20-30%
- **Supports**: Required for some overhangs
- **Print Time**: Approximately 3-5 hours (depends on printer)

## Assembly

1. **Order PCBs** - Use the Gerber files to order PCBs from your preferred manufacturer
2. **Purchase Components** - Refer to the BOM (ibom.html) for the complete parts list
3. **Solder Components** - Start with smaller components (resistors, capacitors) and work up to larger ones
4. **Install Hot-swap Sockets** - Solder the hot-swap sockets for the switches
5. **Flash Firmware** - Program the ESP32 with your custom firmware (firmware not included in this repo)
6. **3D Print Case** - Print the case base and lid
7. **Install Switches** - Insert your favorite mechanical switches into the hot-swap sockets
8. **Final Assembly** - Mount the PCB in the case and attach the lid

## Customization

The HackPad is designed to be fully customizable:

- **Keycaps**: Use any Cherry MX-compatible keycaps
- **Switches**: Hot-swappable - try different switches without soldering
- **RGB Lighting**: Program custom lighting effects
- **Firmware**: Write custom firmware for your specific use case
- **Case**: Modify the 3D model or create your own design

## Design Files

### KiCAD Project Files

Open the project in KiCAD 9.0.7 or later:
- Project file: `JONAHS HACKPAD/JONAHS HACKPAD/PCB Pro Files/PRO/PRO.kicad_pro`
- PCB file: `PRO.kicad_pcb`
- Schematic file: `PRO.kicad_sch`

### 3D Models

- **STEP format**: For CAD software (Fusion 360, SolidWorks, etc.)
- **STL format**: For 3D printing slicers

## Images

### 3D Render
![3D PCB](JONAHS%20HACKPAD/JONAHS%20HACKPAD/KICAD%20Photos/3d%20PCG%20Image.png)

### Case Design
![Case](JONAHS%20HACKPAD/JONAHS%20HACKPAD/FUSION%20Photos/Case.png)
![Lid](JONAHS%20HACKPAD/JONAHS%20HACKPAD/FUSION%20Photos/Lid.png)

## Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests
- Share your builds and modifications

## License

This project is open-source. Please check with the repository owner for specific licensing terms.

## Credits

**Designed by**: Jonah (Kingdragoncat)

## Support

If you build this project or have questions, feel free to open an issue on GitHub!

---

**Enjoy your HackPad!** 🎹✨
