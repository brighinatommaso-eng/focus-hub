# Focus Hub

> 🚧 **Work in progress** — currently in the design phase for [Hack Club Fabricate](https://fabricate.hackclub.com).

Focus Hub is an ESP32-based desk companion that helps me stay focused while studying. It sits on my desk and keeps my timer, my tasks for the day and my notifications in one place, so I don't have to pick up my phone.

## Why I'm building it

I get distracted by my phone every time I study: I unlock it to check the time or a notification and end up scrolling. I wanted a dedicated device that does only the useful parts — timer, to-do list, notifications — and nothing else.

## Features

- **Multiple Pomodoro modes** — classic 25/5, 50/10 and custom intervals, selected with the rotary encoder, with buzzer and LED alerts
- **Daily to-do list** — shown on the display, tasks can be checked off with the encoder and edited from a companion PC app
- **Notifications** — alerts from my PC/phone (Discord, mail, calendar) shown on the display with a color-coded RGB LED
- **Companion PC app** — manages the to-do list, Pomodoro settings and notification forwarding over Wi-Fi

## Hardware

| Part | Purpose |
|---|---|
| ESP32-S3-DevKitC-1 | Main microcontroller, Wi-Fi, native USB |
| 2.4" IPS TFT (ST7789, 240×320) | Timer, tasks, notifications in color |
| EC11 rotary encoder with push button | Menu navigation |
| 2× 6×6 mm tactile buttons | Quick actions |
| 3× APA106 addressable RGB LEDs | Pomodoro progress / notification color |
| Passive buzzer | Timer and notification alerts |
| Custom PCB | Connects everything, mounted with screws |
| 3D printed case | Enclosure |

The full bill of materials with links and prices is in [`BOM.csv`](BOM.csv).

## Images

_Coming soon: 3D model renders, PCB and schematic screenshots._

## Repository structure

```
focus-hub/
├── pcb/        KiCad project (schematic, PCB layout, gerbers)
├── cad/        Case design (.step + Fusion source file)
├── firmware/   ESP32 firmware
├── app/        Companion PC app
├── docs/       Images and documentation
├── BOM.csv     Bill of materials
└── JOURNAL.md  Design journal
```

## How to build it

_Assembly instructions will be added once the design is finished._

## How to flash the firmware

_Coming soon._

## Status

- [ ] Schematic (KiCad)
- [ ] PCB layout (KiCad)
- [ ] Case design (Fusion)
- [ ] Firmware
- [ ] Companion PC app
- [ ] Build and test

## Credits

_Libraries and references used will be listed here._
