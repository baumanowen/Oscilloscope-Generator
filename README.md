# \# STM32 Sine Wave Generator with PWM

# 

# This project uses an STM32 microcontroller to generate a sinusoidal signal using PWM output, filtered through an RC network, with optional signal buffering via an op-amp.

# 

# \## Features

# \- Sine wave generation using a precomputed lookup table

# \- Adjustable amplitude and offset

# \- PWM output via TIM1

# \- RC filter smoothing the PWM to approximate analog output

# \- Real-time ADC sampling displayed over UART

# \- Configurable via STM32CubeMX `.ioc` file

# 

# \## Files

# \- `YourProject.ioc` - STM32CubeMX project configuration

# \- `Core/Src/main.c` - Main application code

# \- `Core/Src/\*` - Other source files

# \- `README.md` - This file

# 

# \## Hardware Requirements

# \- STM32 Nucleo or similar development board

# \- External RC filter on PWM output

# \- Optional: Rail-to-rail op-amp for signal buffering

# 

# \## Usage

# 1\. Open `.ioc` with STM32CubeIDE

# 2\. Generate project files

# 3\. Compile and flash to the STM32

# 4\. Connect UART to serial monitor for ADC data

# 5\. Observe filtered sine output with oscilloscope

# 

# \## Future Improvements

# \- Adjustable frequency via user input

# \- Dynamic sine table generation

