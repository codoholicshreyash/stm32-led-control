# STM32 Nucleo-L64 LED Control

This repository contains a minimal example project that blinks the **LD2 (green) LED** on an STM32 Nucleo‑64 development board, based on the tutorial published by CircuitDigest:  
<https://circuitdigest.com/microcontroller-projects/getting-started-with-stm32-nucleo64-using-stm32cubemx-and-truestudio>

## Hardware

| Board | On‑board LED | GPIO Pin |
|-------|--------------|----------|
| Nucleo‑F401RE / F103RB / F446RE | LD2 (green) | `PA5` |

> *If you are using a different Nucleo‑64 variant, update the pin number in `src/main.c` accordingly.*

## Getting Started

1. **Clone** or download this repository.  
   ```bash
   git clone https://github.com/<your‑username>/stm32‑led‑control.git
   cd stm32‑led‑control
   ```

2. **Import** the project into **STM32CubeIDE** (or TrueSTUDIO):
   - `File → Import… → Existing Projects into Workspace`
   - Browse to the repository root and finish.

3. **Compile & Flash**  
   Click the ▶️ **Run** button or press `Ctrl + F11` to build and program the MCU.  
   The LED should start toggling every 500 ms.

### Re‑generating Code with STM32CubeMX

An `.ioc` file (`stm32_led_control.ioc`) is included so you can open the project in CubeMX, tweak pin assignments or clock settings, and regenerate the HAL code.

## File Structure

```
.
├── .gitignore
├── LICENSE
├── README.md
├── stm32_led_control.ioc
└── src
    └── main.c
```

## License

MIT — see `LICENSE` for details.