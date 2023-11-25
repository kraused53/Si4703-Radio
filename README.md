# Si4703 Radio
> Overview

I started this project to practice my C coding skills, and to learn more about how STM32 peripherals work. It uses an STM32F103 microcontroller and an Si4703 FM module to make a basic desktop radio. I am not setting out to write an fully featured library for the Si4703, I am only implementing functions that I need for this specific project.

# STM32F103
> Overview

I chose this microcontroller because I already had an "STM32 Blue Pill" which uses the STM32F103C8T6.  Ths STM32F103C8T6 is a 32-Bit ARM Cortex-M3 microcontroller that can be clocked up to 72 MHz at 3.3V. I am using 2 I<sup>2</sup>C ports, an SPI port, a UART port and several GPIO pins.

> Hardware
 - Crystal Oscillator
    - High Speed External Clock Source
        - PD1  > HSE Output
        - PD0  > HSE Input
 - Serial Wire Debug
    - Programming Header
        - PA14 > SWCLK
        - PA13 > SWDIO
 - I<sup>2</sup>C 1
    - Si4703
        - PB7  > SDA
        - PB6  > SCL
 - I<sup>2</sup>C 2
    - SSD1306
        - PB11 > SDA
        - PB10 > SCL
 - SPI 2
    - SSD1306
        - PB15 > MOSI
        - PB14 > MISO
        - PB13 > SCK
 - UART 2
    - Interface
        - PA3  > RX
        - PA2  > TX
 - GPIO
    - Interface
        - PB2  > Mono Button
        - PB1  > Mute Button
        - PB0  > Seek Down Button
        - PA7  > Seek Up Button
        - PA6  > Tune Down Button
        - PA5  > Tune Up Button
        - PA4  > Volume Down Button
        - PA1  > Volume Up Button
    - LEDs
        - PA12 > Stereo LED
        - PA11 > Mono LED
        - PA10 > Mute LED
    - SSD1306 ( SPI )
        - PB12 > Reset
        - PA9  > CS
        - PA8  > DS
    - Si4703
        - PB5  > Reset
# Si4703 Module - I<sup>2</sup>C
> Overview

# SSD1306 - SPI
> Overview

# SSD1306 - I<sup>2</sup>C
> Overview

# Interface - GPIO
> Overview

# Interface - UART
> Overview

# PCB
> Overview