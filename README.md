# STM32 Sine Wave Generator Using PWM

This project generates a sinusoidal waveform using PWM on an STM32 microcontroller (e.g., Nucleo board). The PWM output, when filtered with a simple RC low-pass filter, approximates an analog sine wave.

---

## Features

- Generates a 100-sample sine lookup table  
- Uses TIM1 PWM Channel 1 for output  
- Adjustable amplitude and offset parameters  
- Includes UART ADC reading for real-time monitoring  
- Easy to modify and extend for different frequencies or waveforms  

---

## Project Structure

- `.ioc` — STM32CubeMX configuration file  
- `Core/Src/main.c` — Main application source code  
- `README.md` — Project overview and instructions  

---

## How It Works

1. A sine lookup table (`sine_table`) is generated with 100 samples representing one full sine wave cycle.  
2. PWM duty cycle is updated in a loop based on the sine table to output the waveform.  
3. An RC low-pass filter smooths the PWM output to create an analog sine wave approximation.  
4. The ADC continuously reads an input channel and sends the data over UART for monitoring.  

---

## Usage

1. Open the `.ioc` file with STM32CubeIDE and generate project code.  
2. Build and flash the firmware to your STM32 board.  
3. Connect the PWM output pin through an RC low-pass filter (e.g., R = 10kΩ, C = 0.1µF) to observe the sine wave.  
4. Use a serial terminal (baud 115200) to view ADC readings from the UART output.  

---

## Future Improvements

- Add frequency control to change sine wave speed dynamically.  
- Use DAC output for cleaner analog signals instead of PWM + filter.  
- Implement other waveforms (square, triangle) for waveform generator capabilities.  
- Integrate with oscilloscope project for full function generator and scope combo.  

---

## Requirements

- STM32 microcontroller (tested on Nucleo boards)  
- STM32CubeIDE for development  
- Basic RC low-pass filter for analog output  
- UART terminal program for serial monitoring (e.g., PuTTY, Tera Term)  

---

## License

This project is provide
